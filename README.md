# Authcord inc v1

**Authcord inc v1** by **aaa (pyattrz)** is a **fast, async Discord bot** built with **FastAPI**, designed for **member backup and restoration using stored tokens (auths)**. This streamlined version focuses on speed and simplicity.

---

## Features

* :floppy_disk: **Member Backup**: Save Discord members' tokens safely.
* :arrows_counterclockwise: **Member Restoration**: Re-add backed-up members to any server.
* :zap: **Fully Async**: FastAPI-powered for fast operations.
* :tools: **Lightweight**: Minimal and focused on handling auths.
* :shield: **Auto Token Refresh**: Automatic token management for long-term reliability.
* :link: **API Endpoints**: RESTful API for stock management and monitoring.

---

## Installation

```bash
# Clone the repository
git clone https://github.com/pyattrs/AuthCord-Inc.git
cd authcord-inc

# Install dependencies
pip install -r requirements.txt
```

---

## Configuration

Edit `config.json` with your bot details:

```json
{
  "token": "YOUR_BOT_TOKEN",
  "secret": "YOUR_BOT_SECRET",
  "id": "YOUR_BOT_CLIENT_ID",
  "redirect": "http://your-ip:14142/callback",
  "api_endpoint": "https://discord.com/api/v10",
  "webhook": "YOUR_WEBHOOK_URL",
  "guild_ids": ["GUILD_ID_1", "GUILD_ID_2"],
  "role_ids": ["ROLE_ID_1", "ROLE_ID_2"]
}
```

---

## Usage

```bash
# Run the bot
python app.py
```

### Bot Commands

| Command          | Description                      |
| ---------------- | -------------------------------- |
| `/refresh`       | Refresh all stored tokens        |
| `/stock`         | Show current auth stock count    |
| `/pull <server_id> <amount>` | Pull members to specified server |
| `/verify`        | Send verification embed with button |

### API Endpoints

- `GET /` - Check API status
- `GET /stock` - View current stock count
- `POST /add_stock` - Manually add stock (requires user_id, access_token, refresh_token)

---

## Contributing

1. Fork the repository.
2. Create a branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push branch (`git push origin feature-name`).
5. Open a Pull Request.

---

## Disclaimer

**Authcord inc v1** is intended solely for **controlled member backup and restoration**. Misuse for spamming or unauthorized member adding may violate Discord's Terms of Service. Use responsibly and in compliance with Discord's guidelines.
```
The bot now has all the requested functionality with proper error handling and a professional structure!
