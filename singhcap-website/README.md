# Singh Capital Partners

Official website for Singh Capital Partners - a multi-asset family office.

**Intelligent Capital. Enduring Impact.**

## Features

- Modern, sophisticated cream aesthetic
- Cycling background video showcasing portfolio companies (Oats Overnight, SpaceX)
- Interactive portfolio with 100+ companies across Venture, Growth, and Funds
- Detailed company modals with websites and social media links
- Fully responsive design

## File Structure

```
singhcap-website/
├── index.html              # Main website file
├── README.md               # This file
└── videos/                 # Background videos
    ├── oats-overnight.mp4
    └── spacex.mp4
```

## Deployment

### Option 1: GitHub Pages

1. Upload all files to a GitHub repository
2. Go to **Settings** → **Pages**
3. Select branch (usually `main`) and root folder
4. Your site will be live at `https://[username].github.io/[repo-name]/`

### Option 2: Custom Domain

After enabling GitHub Pages, you can connect a custom domain:
1. Add a `CNAME` file with your domain
2. Configure DNS to point to GitHub Pages
3. Enable HTTPS in repository settings

### Option 3: Any Web Host

Simply upload all files (maintaining the folder structure) to any web hosting service.

## Local Preview

To preview locally, open `index.html` in a browser. For full video playback, you may need to run a local server:

```bash
# Python 3
python3 -m http.server 8000

# Node.js
npx serve

# Then visit http://localhost:8000
```

## Adding New Portfolio Videos

To add more videos to the background cycle:

1. Add your `.mp4` file to the `videos/` folder
2. In `index.html`, find the `videoSources` array (near the top of the `<script>` section)
3. Add your video to the array:

```javascript
const videoSources = [
    'videos/oats-overnight.mp4',
    'videos/spacex.mp4',
    'videos/your-new-video.mp4'  // Add here
];
```

## Tech Stack

- Pure HTML5 / CSS3 / Vanilla JavaScript
- No build process or dependencies required
- Inter font from Google Fonts
- Optimized MP4 videos (H.264)

---

© Singh Capital Partners
