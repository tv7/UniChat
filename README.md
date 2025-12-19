UniChat - Unified Streaming Control Center

Version 1.0

UniChat merges your Twitch, Kick, YouTube, and TikTok chats into one professional, clean interface that you can dock directly inside OBS Studio. It supports custom emotes, dark mode, and Twitch replies.

🚀 Quick Start Guide
1. Installation

Run the UniChat.exe application.

Wait for the status light to turn green (Server Ready).

2. Connect Your Platforms

(You only need to do this once. The app saves your keys automatically.)

🟣 Twitch Setup

In the UniChat app, click the small "Get" button next to the Token box.

A browser window will open asking you to authorize the app. Click Authorize.

You will be redirected to a page. Copy the access_token from the URL bar (it looks like a long string of random characters).

Paste it into the Twitch Token box in the app.

Enter your Channel Name (your username) in the second box.

🟢 Kick Setup

Enter your Kick Username.

Note: A hidden browser window will open in the background to read the chat. This is normal.

🔴 YouTube Setup (Required: API Key)

YouTube requires a free API Key to find your live stream automatically.

Go to the Google Cloud Console.

Create a New Project (name it "UniChat").

In the search bar at the top, search for "YouTube Data API v3".

Click on it and click Enable.

Go to Credentials (on the left menu) -> Create Credentials -> API Key.

Copy the key (starts with AIza...) and paste it into the API Key box in UniChat.

Enter your Channel Handle (e.g., @YourName) or Channel ID (UC...) in the second box.

🎵 TikTok Setup

Enter your TikTok Username (e.g., @user).

Note: You must be currently LIVE for this to connect.

3. Launching the Engine

Once your keys are entered, click the big green "START ENGINE" button.

The status light will turn Green and say "Active".

4. Adding to OBS Studio

In the UniChat app, click the "Copy for OBS" button at the bottom.

Open OBS Studio.

In the top menu, go to Docks -> Custom Browser Docks...

Dock Name: UniChat

URL: Paste the link you copied (e.g., http://127.0.0.1:5500).

Click Apply.

A new window will pop up. You can drag and snap this window into your OBS layout!

💡 Pro Tips

Reply to Chat: You can type in the box at the bottom of the OBS dock to reply directly to Twitch chat.

On-Stream Overlay: If you want the chat to appear on top of your game for viewers to see:

Add a Browser Source in OBS.

Check [x] Local File.

Browse and select the index.html file located in your UniChat folder.

Set Width: 400, Height: 800.

🛠️ Troubleshooting

"The chat page keeps loading..."

Make sure you clicked START ENGINE in the app.

Ensure no other instances of UniChat are running in the background.

"YouTube chat isn't showing up..."

Make sure you are currently LIVE. The API cannot connect to a stream that hasn't started.

Double-check your API Key in the Google Cloud Console.

"Kick chat stopped working..."

Kick sometimes blocks automated tools. Restart the engine to launch a fresh browser session.
