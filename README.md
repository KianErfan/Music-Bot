# Discord Music Bot 🎵

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](#license)
[![Python](https://img.shields.io/badge/python-3.6%2B-3670A0?logo=python&logoColor=ffdd54)](https://www.python.org/downloads/)
[![Discord.py](https://img.shields.io/badge/discord.py-1.5.1-%237289DA?logo=discord&logoColor=white)](https://discordpy.readthedocs.io/)
[![Lavalink](https://img.shields.io/badge/Lavalink-3.1.3-13aa52?logo=node.js&logoColor=white)](https://github.com/Frederikam/Lavalink)

A feature-rich Discord music bot built with Python, Discord.py, and Lavalink. Stream high-quality audio from YouTube, manage playlists, and control playback with intuitive commands.

## Features ✨
- High-quality audio streaming via Lavalink
- Playlist management with queue system
- Track selection interface with reactions
- Playback controls (play, pause, skip, stop)
- Queue shuffling and repeat modes
- Voice channel auto-cleanup when empty
- Customizable prefix and configurations

## Setup Guide 🚀

### Prerequisites
1. Python 3.6+ (recommended 3.8+)
2. Discord Bot Token ([create here](https://discord.com/developers/applications))
3. Lavalink server ([deploy guide](#lavalink-setup))
4. FFmpeg installed and in PATH

### Installation
```bash
git clone https://github.com/KianErfan/Music-Bot.git
cd Music-Bot
python -m pip install -r requirements.txt
```

### Configuration
1. Create token.0 file with your bot token:
  `YOUR_DISCORD_BOT_TOKEN`

2. Configure Lavalink server details in bot.py:
```bash
   nodes = {
    "MAIN": {
        "host": "YOUR_LAVALINK_HOST",
        "port": 2333,
        "rest_uri": "http://YOUR_LAVALINK_HOST:2333",
        "password": "YOUR_LAVALINK_PASSWORD",
        "identifier": "MAIN",
        "region": "europe",
    }

}
```

3. Running the Bot
  `python launcher.py`

### Commands
| Command | Aliases | Description | Example |
|---|---|---|---|
| `?play` | - | Play a song or resume playback | `?play Believer` |
| `?connect` | `join` | Join voice channel | `?connect` |
| `?disconnect` | `leave` | Leave voice channel | `?leave` |
| `?pause` | - | Pause playback | `?pause` |
| `?stop` | - | Stop playback and clear queue | `?stop` |
| `?next` | `skip` | Skip current track | `?skip` |
| `?previous` | - | Play previous track | `?previous` |
| `?shuffle` | - | Shuffle the queue | `?shuffle` |
| `?repeat` | - | Set repeat mode [none/1/all] | `?repeat all` |
| `?queue` | - | Show current queue | `?queue 5` |

### License
Distributed under the MIT License. See `LICENSE` for more information.




