# Streaming room in Node.js, rtmp, hsl, html5
Fully operational server and client for streaming and playing.

## Features
**Server:**
- Has a **rtmp server** to receive streaming (e.g. from OBS studio)
- Converts **rtmp** ro **hsl** when a **rtmp** is published
- WebSocket server for counting participants
- Simple room authentication

**Client:**
- HTML5 VideoJS player (supports Chrome, Firefox, iOS, Android)
- Chat room with usernames
- Password protected

# How it works
Example:

**[ OBS ]** ––rtmp://localhost/live/live––> **[ RTMP Server ]** ––hsl––> **[ HTTP server ]** ––.m3u8––> **[ Videojs HTML5 player ]**

# Requirements
1. ## Nodejs
    *For web and rtmp server*

    Download here: https://nodejs.org/en/download/

2. ## FFmpeg
    *For converting video and audio to HLS (HTML5)*

    Download here: http://ffmpeg.zeranoe.com/builds/


# How to use it
Clone this repository or download the folder.

Open the project folder in <u>terminal</u> and run:

```sh
npm install
```

```sh
npm start
```

Open you browser in `localhost:3000`

- **Username:** [Anything]
- **Password:** room1

You can update the default password in `passwords.json`

### Development
```sh
npm run dev
```
