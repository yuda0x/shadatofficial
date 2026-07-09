# 🎬 Live Streaming by Shakil

A modern, responsive IPTV player built with pure HTML, CSS, and JavaScript. Deploy on Vercel with zero backend required!

## ✨ Features

- 📱 Fully responsive design (Desktop, Tablet, Mobile)
- 🎥 Multi-format support (HLS, DASH, MP4, MPEGTS)
- 🌙 Dark/Light theme toggle
- ⭐ Favorite channels bookmark
- 🔍 Real-time channel search
- 🎚️ Quality selection (auto, 720p, 1080p, 4K)
- 🔊 Volume control & keyboard shortcuts
- 🖼️ Picture-in-Picture mode
- ⌨️ Fullscreen support
- 🔒 Playback lock feature
- 📊 Signal quality indicator

## 📁 File Structure

```
your-repo/
├── index.html        (Main player - 0 backend dependencies)
├── channels.json     (Your streaming channels)
├── vercel.json       (Deployment config)
└── README.md         (This file)
```

## 🚀 Quick Start

### Option 1: Deploy on Vercel (Recommended)

1. **Fork/Clone this repo to GitHub**
   ```bash
   git clone https://github.com/yourusername/your-repo.git
   cd your-repo
   ```

2. **Update `channels.json` with your streams**
   ```json
   {
     "channels": [
       {
         "id": 1,
         "name": "Channel Name",
         "category": "Sports",
         "logo": "https://example.com/logo.png",
         "url": "https://stream-url.com/stream.m3u8",
         "qualityVariants": []
       }
     ]
   }
   ```

3. **Deploy to Vercel**
   - Go to [vercel.com](https://vercel.com)
   - Click "New Project"
   - Select your GitHub repository
   - Click "Deploy"
   - Done! ✅

### Option 2: Local Development

```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js (with http-server)
npx http-server

# Then visit: http://localhost:8000
```

## 📝 Adding Channels

Edit `channels.json`:

```json
{
  "channels": [
    {
      "id": 1,
      "name": "BTV World",
      "category": "Bangla",
      "logo": "https://example.com/btv-logo.png",
      "url": "https://example.com/btv.m3u8",
      "qualityVariants": []
    },
    {
      "id": 2,
      "name": "Sports HD",
      "category": "Sports",
      "logo": "https://example.com/sports-logo.png",
      "url": "https://example.com/sports.m3u8",
      "qualityVariants": []
    }
  ]
}
```

### Stream URL Formats Supported:
- **HLS**: `https://example.com/stream.m3u8`
- **MP4**: `https://example.com/video.mp4`
- **DASH**: `https://example.com/stream.mpd`
- **MPEGTS**: `https://example.com/stream.ts`

### Categories Available:
- Sports
- Bangla
- Movies
- Music
- News
- Entertainment
- Kids
- General

## ⌨️ Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `Space` or `K` | Play/Pause |
| `M` | Mute/Unmute |
| `F` | Fullscreen |
| `R` | Refresh |
| `←` | Seek -10s |
| `→` | Seek +10s |
| `↑` | Volume +10% |
| `↓` | Volume -10% |

## 🎨 Customization

### Change App Title
Edit `index.html`:
```html
<title>Your App Name</title>
```

And update header:
```html
<h2>Your App Name</h2>
```

### Change Telegram Link
Update in `index.html`:
```html
<a href="https://t.me/yourusername" ...>Join</a>
```

### Change Colors
Edit CSS variables in `<style>`:
```css
:root {
  --brand: #2b7de9;      /* Primary color */
  --danger: #e54444;     /* Error/Danger color */
  --success: #22c55e;    /* Success color */
}
```

## 📱 Responsive Breakpoints

- **Mobile**: < 768px
- **Tablet**: 768px - 1024px
- **Desktop**: > 1024px

## 🔧 Technical Details

### No Backend Required
- ✅ Loads channels from static `channels.json`
- ✅ No server-side API calls
- ✅ No database needed
- ✅ Works on any static hosting

### Libraries Used
- **HLS.js** - HLS streaming
- **mpegts.js** - MPEGTS streaming
- **Shaka Player** - DASH streaming
- **Font Awesome** - Icons
- **Google Fonts (Nunito)** - Typography

### Browser Support
- Chrome/Edge 60+
- Firefox 55+
- Safari 11+
- iOS Safari 11+
- Android Chrome 60+

## 📊 Performance

- **Page Load**: < 500ms
- **Player Ready**: < 1s
- **Minified HTML**: ~45KB
- **No external dependencies** (CDN hosted libraries only)

## 🐛 Troubleshooting

### Streams not playing?
1. Check if stream URL is accessible
2. Verify CORS headers are set
3. Try different stream format (HLS/MP4/DASH)
4. Check browser console for errors

### Channels not loading?
1. Ensure `channels.json` is in root directory
2. Check JSON syntax (use [jsonlint.com](https://jsonlint.com))
3. Verify file paths are correct
4. Check browser network tab

### Playback issues?
1. Refresh the page
2. Clear browser cache
3. Try different video quality
4. Check internet connection speed

## 📄 License

Free to use and modify for personal/commercial projects.

## 🤝 Support

- **Telegram**: https://t.me/shakilofficial69
- **Issues**: Open an issue on GitHub
- **Questions**: Comment on repository

## 🎯 Roadmap

- [ ] EPG (Electronic Program Guide)
- [ ] Recording feature
- [ ] Chromecast support
- [ ] Android app
- [ ] Playlist management UI
- [ ] DVR functionality

## 📈 Stats

- ⭐ Star this repo if you find it useful!
- 📢 Share with friends
- 🐛 Report bugs
- 💡 Suggest features

---

**Made with ❤️ by Shakil**  
Last Updated: 2026

