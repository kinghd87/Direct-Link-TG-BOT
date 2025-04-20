# Direct-Link-TG-BOT

A simple and efficient Telegram bot built with Python and the `pyTelegramBotAPI` library that allows users to upload files and receive direct download links. The bot also supports broadcasting messages and managing users by an authorized admin.

---

## Features

- **User Registration:** Users join the bot using `/start` or `/join` commands and get registered automatically.
- **File Upload & Sharing:** Users can send documents, photos, audio, video, and animations to the bot and receive a direct download link.
- **File Forwarding:** Uploaded files are forwarded to a specified Telegram channel for centralized storage.
- **Broadcast Messages:** Authorized user can broadcast messages or media to all registered users.
- **User Management:** Admin can retrieve the list of users and load users from a formatted message.
- **Persistent User Data:** User data is saved in a JSON file (`bot_users.json`) for persistence across restarts.

---

## Prerequisites

- Python 3.7+
- `pyTelegramBotAPI` library

---

## Installation

1. **Clone the repository:**
2. **Install dependencies:**
3. **Configure the bot:**

Open the main script and update the following variables with your own values:

1. TOKEN = "YOUR_BOT_TOKEN"
2. CHANNEL_ID = "YOUR_CHANNEL_ID"
3. AUTHORIZED_USER_ID = YOUR_TELEGRAM_USER_ID

### Commands

- `/start` or `/join`  
  Register yourself as a bot user and get a welcome message.

- `/broadcast` (Admin only)  
  Broadcast a message or media to all registered users. Use this command as a reply to the message you want to broadcast.

- `/get_users` (Admin only)  
  Retrieve a list of all registered users.

- `/load_users` (Admin only)  
  Load users from a formatted message. Use this command as a reply to a message containing a user list.

---

## How It Works

1. Users start the bot and register themselves.
2. Users send files (documents, photos, audio, video, animations) to the bot.
3. The bot forwards the files to a designated Telegram channel.
4. The bot replies with a direct download link to the uploaded file.
5. The authorized admin can broadcast messages or manage users.
---




