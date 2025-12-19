Below is a clean, well-structured **README.md** you can drop straight into GitHub.
I kept it practical, skimmable, and GitHub-friendly.
I also added the **Support my Work** link as requested.

---

# UniChat – Unified Streaming Control Center

**UniChat** brings Twitch, Kick, YouTube, and TikTok chat into one interface.
You dock it directly inside OBS Studio.
You get a clean layout, dark mode, custom emotes, and Twitch replies.

Version: **1.0**

---

## Features

* One chat for Twitch, Kick, YouTube, TikTok
* OBS dock support
* Twitch replies from OBS
* Custom emotes
* Dark mode
* Lightweight local server

---

## Requirements

* Windows
* OBS Studio
* Active streaming accounts on supported platforms

---

## Quick Start

### 1. Install

1. Run `UniChat.exe`
2. Wait for the status light to turn **green** (Server Ready)

---

### 2. Connect Platforms

You only do this once.
UniChat saves your keys automatically.

---

#### Twitch Setup

1. Click **Get** next to the Token field
2. Authorize the app in your browser
3. Copy `access_token` from the URL bar
4. Paste it into the Twitch Token field
5. Enter your **channel name**

---

#### Kick Setup

1. Enter your **Kick username**

Notes:

* A hidden browser window opens in the background
* This is expected behavior

---

#### YouTube Setup (API Key Required)

YouTube needs an API key to detect your live stream.

Steps:

1. Open Google Cloud Console
2. Create a new project (example: `UniChat`)
3. Enable **YouTube Data API v3**
4. Go to **Credentials → Create Credentials → API Key**
5. Copy the key (starts with `AIza`)
6. Paste it into UniChat
7. Enter your **channel handle** (`@name`) or **channel ID** (`UC...`)

---

#### TikTok Setup

1. Enter your **TikTok username** (example: `@user`)

Notes:

* You must be **live** for TikTok chat to connect

---

### 3. Start the Engine

1. Click **START ENGINE**
2. Status light turns **green**
3. Engine status shows **Active**

---

## Add UniChat to OBS

1. Click **Copy for OBS** in UniChat
2. Open OBS Studio
3. Go to **Docks → Custom Browser Docks**
4. Set:

   * Dock Name: `UniChat`
   * URL: paste copied link (example: `http://127.0.0.1:5500`)
5. Click **Apply**
6. Dock the window anywhere in OBS

---

## On-Stream Chat Overlay (Optional)

To show chat to viewers:

1. In OBS, add a **Browser Source**
2. Enable **Local File**
3. Select `index.html` from the UniChat folder
4. Set:

   * Width: `400`
   * Height: `800`

---

## Pro Tips

* Type in the dock input to reply to Twitch chat
* Restart the engine if a platform disconnects
* Keep UniChat running before launching OBS

---

## Troubleshooting

### Chat page keeps loading

* Click **START ENGINE**
* Close duplicate UniChat instances

### YouTube chat not showing

* You must be **live**
* Recheck your API key

### Kick chat stopped

* Restart the engine
* Kick blocks sessions at times

---

## Support My Work

If UniChat helps your stream, you can support development here:

👉 **[https://linkhub-pro.netlify.app/](https://linkhub-pro.netlify.app/)**

---

## License

Free for personal streaming use.

---

Created for streamers who want one chat, not four.
