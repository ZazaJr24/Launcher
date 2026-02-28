# Gamers Unlimited Launcher
[
[
[

**The ultimate game launcher for premium titles**  
A modern, fast, and user-friendly launcher for 40+ current AAA games. Supports downloads, resuming, pausing, and live settings without restart.

## 🎮 Features

| **Feature** | **Status** |
|-------------|------------|
| **40+ Premium Games** | Assassin's Creed, EA FC 24-26, Black Myth Wukong, Dragon's Dogma 2 & more |
| **Multi-Part Downloads** | Automatic sequence (part1 → part2 → ...) |
| **Resume & Pause** | Pause/resume downloads anytime |
| **Live Theme Switching** | 6 themes (Dark, Light, Ocean, Forest, Purple, Sunset) |
| **Card Sizes** | Small/Medium/Large (live preview) |
| **Download Position** | Bottom/Right Sidebar |
| **Timeout Protection** | No crashes on slow connections |
| **Auto-Update** | GitHub releases with taskbar flash |
| **Multi-Language** | EN, DE, FR, ES, AR |

## 🚀 Installation

### Windows (recommended)
1. **Download** the latest `.exe` from [Releases](https://github.com/ZazaJr24/Launcher/releases/latest)
2. **Run** → no installation required
3. **First start** → choose download folder

### Developers
```bash
git clone https://github.com/ZazaJr24/Launcher.git
cd Launcher
pip install -r requirements.txt
python launcher.py
```

## 📦 Requirements
```txt
Python 3.8+
tkinter (standard)
Pillow (for rounded cards)
requests (optional)
```

## ⚙️ Configuration

All settings are automatically saved to `launcher_config.json`:

```json
{
  "current_theme": "dark",
  "card_size": "medium", 
  "download_display": "bottom",
  "download_box_height": 180,
  "language": "English",
  "paused_download": null
}
```

## 🎨 Themes

| **Theme** | **Main Color** |
|-----------|----------------|
| `dark` | #0A84FF |
| `light` | #888888 |
| `ocean` | #00C2FF |
| `purple` | #A855F7 |
| `forest` | #22C55E |
| `sunset` | #FF6B35 |

## 🕹️ Supported Games (selection)

| **Title** | **Parts** | **Status** |
|-----------|-----------|------------|
| Assassin's Creed Shadows | 13 | ✅ |
| Black Myth: Wukong | 14 | ✅ |
| EA FC 26 | 7 | ✅ |
| Monster Hunter Wilds | 8 | ✅ |
| Stellar Blade | 6 | ✅ |
| Street Fighter 6 | 10 | ✅ |

**→ Full list**: 40+ titles in launcher

## 🔧 Technical Features

### Performance Optimizations
```
✅ Timeout protection (5s requests)
✅ Widget image caching  
✅ Threaded downloads
✅ Live UI without restart
✅ Auto-resume on crashes
```

### Theme System
- **6 Themes** with individual color palettes
- **Live switching** without restart
- **Widget reference cleanup** → no "bad window path name"

## 🤝 Contributing

1. **Fork** this repository
2. **New branch** `git checkout -b feature/xyz`
3. **Commit** changes `git commit -m "Add: XYZ"`
4. **Push** `git push origin feature/xyz`
5. **Create Pull Request**

### Adding new games
```python
GAME_CONTENT_IDS["New Game"] = [
    ("uuid1", "DataPackage_New.part1.rar"),
    ("uuid2", "DataPackage_New.part2.rar")
]
```

## 📄 License
MIT License - see [LICENSE](LICENSE) © 2026 Gamers Unlimited

## 🙏 Thanks
- **Ubisoft, EA, Capcom** for the great games
- **Tkinter & PIL** for the stable foundation
- **Community** for feedback & bug reports

***

**⭐ Star this repo if you like the launcher!**

> **Made with ❤️ for real gamers**  
> *February 2026 - ZazaJr24*
For educational Purpose only
