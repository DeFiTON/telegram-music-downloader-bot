# 🎵 Telegram Music Downloader Bot

A powerful and user-friendly Telegram bot that allows users to download music from various sources with support for multiple formats and high-quality audio.

## ✨ Features

- 🎧 Download music from popular platforms (YouTube, SoundCloud, etc.)
- 🎵 Multiple audio format support (MP3, FLAC, WAV)
- 📋 Playlist and album download support  
- 🔍 Search functionality for finding specific tracks
- 📁 Organized file management and metadata tagging
- 👥 User-friendly inline keyboard interface
- ⚡ Fast and reliable downloads
- 🌍 Multi-language support

## 🛠️ Requirements

### System Requirements
- Python 3.8 or higher
- Linux/Windows/macOS
- At least 1GB RAM
- Stable internet connection

### Python Dependencies
```bash
pip install python-telegram-bot
pip install yt-dlp
pip install requests
pip install aiohttp
pip install mutagen
pip install asyncio
```

### External Dependencies
- FFmpeg (for audio processing)
- Git (for cloning the repository)

## 🚀 Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/DeFiTON/telegram-music-downloader-bot.git
cd telegram-music-downloader-bot
```

### 2. Install Dependencies
```bash
# Install Python dependencies
pip install -r requirements.txt

# Install FFmpeg
# Ubuntu/Debian:
sudo apt update && sudo apt install ffmpeg

# macOS:
brew install ffmpeg

# Windows: Download from https://ffmpeg.org/download.html
```

### 3. Configuration
1. Create a new bot via [@BotFather](https://t.me/BotFather) on Telegram
2. Copy your bot token
3. Create a `.env` file in the project root:
```env
BOT_TOKEN=your_bot_token_here
ADMIN_ID=your_telegram_user_id
DOWNLOAD_PATH=./downloads/
MAX_FILE_SIZE=50
```

### 4. Running the Bot
```bash
# Development mode
python bot.py

# Production mode with process manager
pm2 start bot.py --name music-bot
```

## 📖 Usage

### Basic Commands
- `/start` - Initialize the bot
- `/help` - Show available commands
- `/search <query>` - Search for music
- `/download <url>` - Download from URL
- `/settings` - Configure bot settings
- `/stats` - Show download statistics

### Supported URLs
- YouTube: `https://youtube.com/watch?v=...`
- YouTube Music: `https://music.youtube.com/...`
- SoundCloud: `https://soundcloud.com/...`
- Spotify: `https://open.spotify.com/...` (requires premium)

## 🔧 Configuration Options

Edit the `config.py` file to customize:
- Download quality settings
- File format preferences
- Rate limiting parameters
- Storage locations
- Supported platforms

## 📁 Project Structure
```
telegram-music-downloader-bot/
├── bot.py              # Main bot file
├── config.py           # Configuration settings
├── handlers/           # Command and callback handlers
├── utils/              # Utility functions
├── downloads/          # Downloaded files directory
├── requirements.txt    # Python dependencies
├── .env.example        # Environment variables template
└── README.md           # This file
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/new-feature`
3. Commit your changes: `git commit -am 'Add new feature'`
4. Push to the branch: `git push origin feature/new-feature`
5. Submit a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⚠️ Disclaimer

This bot is for educational purposes only. Please respect copyright laws and terms of service of the platforms you download from. Users are responsible for ensuring they have the right to download and use the content.

## 🆘 Support

If you encounter any issues or have questions:
- Open an [issue](https://github.com/DeFiTON/telegram-music-downloader-bot/issues) on GitHub
- Check the [wiki](https://github.com/DeFiTON/telegram-music-downloader-bot/wiki) for detailed documentation
- Join our [Telegram support group](https://t.me/musicbothelp)

## 🏆 Credits

- Built with [python-telegram-bot](https://python-telegram-bot.org/)
- Uses [yt-dlp](https://github.com/yt-dlp/yt-dlp) for downloading
- Audio processing with [FFmpeg](https://ffmpeg.org/)

---

⭐ **If you find this project useful, please consider giving it a star!** ⭐
