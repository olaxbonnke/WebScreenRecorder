# Web-Record tool 🎥

> **Cinematic Website Video Recorder & Animation Capture Suite.**
> Capture smooth scrolling videos, product demos, and animated hero sections from any URL with multi-engine API support, customizable hero hold duration, and HTML5 video autoplay.

[![Made with Love by Bonnke](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20by-Bonnke-d9a441?style=for-the-badge&logo=vercel)](https://bonnke-dev.vercel.app/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](LICENSE)
[![Deployment: Vercel](https://img.shields.io/badge/Deploy-Vercel-black?style=for-the-badge&logo=vercel)](https://webrecordtool.vercel.app/)

---

## 🌟 Highlights & Features

- ⏱️ **In-Video Hero Hold Duration**: Set a precision pause (e.g. 2s, 3s, 5s) at the top of the page so hero reels, lottie animations, and key headlines play on camera before scrolling down.
- 🎬 **HTML5 Video Autoplay Override**: Automatically wakes up, un-mutes, and loops `<video>` background reels that headless browsers normally suppress.
- 🌐 **Multi-Engine API Architecture**: Seamlessly switch between **ScreenshotOne**, **ScreenshotCore**, **Microlink**, **Urlbox**, and **Custom Self-Hosted / Playwright / Browserless** endpoints.
- 🌓 **Dark & Light Mode**: High-contrast theme toggle with retro-modern aesthetic, persistent preferences, and smooth transitions.
- ✨ **Interactive Particle Canvas**: Subtle mouse-reactive particle grid in background space.
- 📱 **Multi-Device Viewports**: Pre-configured viewports for Desktop ($1440 \times 900$), Tablet ($768 \times 1024$), Mobile ($390 \times 844$), and custom pixel dimensions.
- 🎞️ **Multi-Format Export**: Export recordings to **MP4**, **WebM**, **GIF**, and **MOV**.
- 📊 **Visual Playback Timeline**: Real-time breakdown of video duration ($\text{Hero Hold} \rightarrow \text{Smooth Scroll} \rightarrow \text{Settle/Scroll Back}$).
- 🛡️ **Intelligent Cleanup**: Built-in toggles to block ads, cookie banners, chat widgets, and trackers.
- 💾 **Local Storage Persistence**: Safely caches your API keys and configuration in private browser storage—never sent anywhere except the rendering provider.
- 🚀 **SEO & Vercel Ready**: Comes with `robots.txt`, `sitemap.xml`, OpenGraph metadata, Twitter cards, and Schema.org JSON-LD structured data for Google Search Console indexation.

---

## 🛠️ Supported API Engines

| Engine | Ideal For | Key Capabilities |
| :--- | :--- | :--- |
| **ScreenshotOne** | **Recommended for Hold + Scroll** | Native `scroll_start_delay`, custom scroll easing, signed HMAC requests, ad/cookie blocking. |
| **ScreenshotCore** | High-volume automated recording | Native `video_scroll`, custom FPS, pre-capture delay, direct query authentication. |
| **Microlink** | Quick public/pro testing | Free-tier video recording without keys, `waitForTimeout` support. |
| **Urlbox** | Enterprise rendering | Direct MP4/WebM video generation, HMAC secret signing, full viewport emulation. |
| **Custom / Self-Hosted** | Puppeteer / Playwright / Node | Configurable URL template supporting `{{url}}`, `{{hero_hold_ms}}`, `{{duration}}`, `{{key}}`, etc. |

---

## 🚀 Quick Start (Local Setup)

### 1. Clone the repository
```bash
git clone https://github.com/olaxbonnke/WebScreenRecorder.git
cd WebScreenRecorder
```

### 2. Run with any local server
Because Web-Record tool is built as a zero-dependency static web application, you can run it with Python, Node, or VS Code Live Server:

```bash
# Using Python
python -m http.server 3000

# Or using npx serve
npx serve .
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## 📖 How to Use

1. **Configure Your API Key**:
   - Click the **API Setup** button in the top right.
   - Choose your provider (**ScreenshotOne**, **ScreenshotCore**, **Microlink**, **Urlbox**, or **Custom**).
   - Paste your API key (stored securely in your browser's private local storage).
2. **Enter Website URL**:
   - Type or paste the target URL (e.g. `https://stripe.com` or `https://apple.com`).
3. **Set Hero Hold Duration**:
   - Choose how long the video should hold still at the top hero section ($0\text{s}$ to $15\text{s}$) to let background videos or animations play.
4. **Choose Viewport & Duration**:
   - Pick Desktop, Tablet, Mobile, or Custom resolution.
   - Adjust the total video duration slider.
5. **Hit ● Record Video**:
   - Watch the live viewfinder status.
   - Download the generated video or open the direct high-resolution link.

---

## ☁️ Deploying to Vercel

1. Push your repository to GitHub:
   ```bash
   git add .
   git commit -m "Update app branding to Web-Record tool"
   git push origin main
   ```
2. Go to [vercel.com](https://vercel.com) and click **"Add New Project"**.
3. Import your `WebScreenRecorder` repository.
4. Framework Preset: **Other / Static HTML**.
5. Click **Deploy**.

---

## 🔍 Google Search Console & SEO Submission

This project includes pre-built SEO assets for top search engine visibility:

1. **Verify Ownership**:
   - Go to [Google Search Console](https://search.google.com/search-console).
   - Add your live Vercel domain (e.g. `https://webrecordtool.vercel.app/`).
   - Complete HTML tag verification or DNS verification.
2. **Submit Sitemap**:
   - In Search Console, navigate to **Sitemaps** on the left menu.
   - Enter `sitemap.xml` and click **Submit**.
3. **Test Robots.txt**:
   - Verify `https://webrecordtool.vercel.app/robots.txt` is accessible and returns `Allow: /`.

---

## 👨‍💻 Author & Attribution

Crafted with ❤️ by **Bonnke**

- 🌐 **Portfolio**: [https://bonnke-dev.vercel.app/](https://bonnke-dev.vercel.app/)
- 🐙 **GitHub Profile**: [@olaxbonnke](https://github.com/olaxbonnke)
- ⭐ **Repository**: [WebScreenRecorder on GitHub](https://github.com/olaxbonnke/WebScreenRecorder)

---

## 📄 License

MIT License © 2026 Bonnke. Free to use and modify for personal and commercial projects.
