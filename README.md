# Telegram Sales Bot

A Telegram bot for product sales, order management, and referrals — with separate flows for customers, employees, and admins.

---

## Stack

- [Python](https://www.python.org/)
- [Aiogram](https://docs.aiogram.dev/) — async Telegram Bot framework
- [SQLAlchemy](https://www.sqlalchemy.org/) — ORM and database toolkit
- [bitcoinlib](https://bitcoinlib.readthedocs.io/) — BTC/LTC transaction handling
- [bip-utils](https://github.com/ebellocchia/bip_utils) — HD wallet derivation

---

## Customer menu

| Option | Description |
|---|---|
| **Choose city** | Select city → product → quantity → confirm. Sends product photo and delivery data if balance is sufficient, otherwise prompts a deposit. |
| **Profile** | Account overview and current balance. |
| **Deposit money** | Fund your account via BTC or LTC. |
| **Refresh balance** | Syncs the latest deposits. Rate-limited to once every 30 seconds. |
| **Bonuses** | Referral dashboard: earnings, referral count, and personal link. Earns 10% of each referral's first 5 purchases. |
| **Purchase history** | Past orders with product details. |
| **Info** | App details, terms, and usage instructions. |
| **Support** | Opens a line to the admin. |
| **Choose language** | Switch the interface language. |

---

## Admin menu

Access with `/admin`.

| Option | Description |
|---|---|
| **Broadcast** | Send a message to all users, auto-translated to each user's selected language. |
| **Download database** | Export the full database as a CSV file. |
| **Refund menu** | Review and process pending refund requests. |
| **Statistics** | Purchase and registration counts over the last 1, 7, and 30 days. |
| **Manage categories** | Add or remove categories; configure product photo, name, description, and price. |
| **Manage cities** | Add or remove cities. |
| **Manage balances** | View and edit individual user balances. |
| **Employee management** | Create employee accounts with auto-generated passwords. |
| **Withdraw** | Pull BTC or LTC from all wallets. |
| **Notifications** | Real-time alerts for new deposits (including deposit address and wallet seed) and new purchases. |

---

## Employee menu

Access with `/orderupload <password>`.
Select a city and category, then upload the product photo and delivery data for that order.

## Source Code

https://www.patreon.com/posts/telegram-sales-155348711