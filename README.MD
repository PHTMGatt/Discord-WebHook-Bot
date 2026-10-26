<h1 align="center">🪝 Captain Hook: WebHook Bot</h1>

<p align="center">
  <img src="https://raw.githubusercontent.com/PHTMGatt/12-React-Portfolio/a2c43d8301679dbda14ad06dc225d61e5515e431/src/assets/project-images/Captain%20Hook.png" alt="Captain Hook portfolio artwork" width="800" />
</p>

<p align="center">
  A smart and lightweight GitHub → Discord bot that formats push commit messages using GPT and posts them in your server using a WebHook — no token or bot login needed.
</p>

---

## 💡 What It Does

When someone pushes to GitHub:

```
🪝 Bryen pushed: Updated docs and polished CSS layout
```

Captain Hook formats and posts the commit message directly into your selected Discord channel.

---

## ⚙️ Setup Instructions

### 1. Register Your Repo + Discord WebHook

Visit the registration form:
```
https://discord-webhook-bot-1f23.onrender.com/register
```

You'll be asked to provide:
- Your GitHub username
- Your GitHub repository name
- Your Discord WebHook URL

---

### 2. Add a WebHook to GitHub

1. In your GitHub repo: go to **Settings → Webhooks**
2. Click **Add Webhook**
3. Use this as the **Payload URL**:
```
https://discord-webhook-bot-1f23.onrender.com/github
```
4. Content type: `application/json`
5. Event: **Just the push event**

---

## 📸 Demo

<p align="center">
  <img src="./images/BotUsage.webp" alt="Captain Hook Bot Demo" width="450" />
</p>

---

## ⚙️ Optional `.env` (for local dev or personal hosting)

```env
DISCORD_WEBHOOK_URL=https://discord.com/api/webhooks/your_webhook
OPENAI_API_KEY=sk-...
```

The API key enables GPT formatting. Without it, the bot falls back to local message cleanup.

---

## 🧠 Features

- 🪝 Register any GitHub repo + Discord WebHook
- 💬 Sends clean commit messages on push
- 🤖 GPT-powered cleanup (optional)
- 🌐 Works on Render or locally

---

<p align="center" style="font-size: 0.9rem; color: #666;">
  Developed and maintained by <strong>Bryen Gatt</strong> • MIT License
</p>
