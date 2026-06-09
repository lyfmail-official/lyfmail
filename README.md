# LYF Mail — Privacy-First Digital Wellness Platform

**Every Choice Shapes Tomorrow**

[LYF Mail](https://lyfmail.com) is a privacy-first digital wellness platform based in **Varanasi, Uttar Pradesh, India**. Since 2020, we have delivered free curated newsletters and open-source tools to **50,000+ subscribers across India** — helping people make better decisions about their health, wealth, career, and mental wellbeing.

This repository contains the official **Progressive Web App (PWA)** for LYF Mail. Install it on any device for instant access to newsletters, tools, and insights — no app store required.

---

## 🏠 Main Website
**[https://lyfmail.com](https://lyfmail.com)** — Free weekly newsletters for health, wealth, career, creativity & mindfulness

## 📚 Pillar Guides
- [Health & Wellness Guide](https://lyfmail.com/health-wellness-guide)
- [Personal Finance Guide](https://lyfmail.com/personal-finance-guide)
- [Career Development Guide](https://lyfmail.com/career-development-guide)
- [Creativity Resources](https://lyfmail.com/creativity-resources)
- [Mindfulness Practices](https://lyfmail.com/mindfulness-practices)

## 🛠️ Free Open-Source Tools by LYF Mail

| Tool | Description | Live App |
|------|-------------|----------|
| **TrustLens** | Detect misinformation before you share. Privacy-first credibility analysis. | [trustlens.lyfmail.com](https://trustlens.lyfmail.com) |
| **LYF SOS** | Emergency safety app. Works without internet. Built for India. | [lyfsos.lyfmail.com](https://lyfsos.lyfmail.com) |
| **PDPR** | Public Dark Pattern Registry. Document deceptive UX ethically. | [pdpr.lyfmail.com](https://pdpr.lyfmail.com) |
| **Ebb** | Privacy-first period tracker. Homomorphic encryption. Your data stays yours. | [ebb.lyfmail.com](https://ebb.lyfmail.com) |
| **Together** | Community mental health support. Shared therapeutic silence. | [together.lyfmail.com](https://together.lyfmail.com) |
| **Rewriter** | AI-powered narrative therapy and health content writing assistant. | [lyfmail-official.github.io/rewriter](https://lyfmail-official.github.io/rewriter/) |
| **Offload** | Stress relief tool. Binaural beats, dream journal, zero cloud storage. | [lyfmail-official.github.io/offload](https://lyfmail-official.github.io/offload/) |
| **Signals** | Privacy-first analytics. Human vs. bot detection without cookies. | [signals.lyfmail.com](https://signals.lyfmail.com) |

## 📰 Newsletters
- [Health & Wellness](https://health.signup.lyfmail.com)
- [Personal Finance](https://financing.signup.lyfmail.com)
- [Career Development](https://career.signup.lyfmail.com)
- [Creativity & Innovation](https://creativity.signup.lyfmail.com)
- [Personal Development](https://intuition.signup.lyfmail.com)

## 📖 Documentation
[docs.lyfmail.com](https://docs.lyfmail.com) — Technical guides, API references, and contribution guidelines

## 🤝 Support
- [support.lyfmail.com](https://support.lyfmail.com)
- contact@lyfmail.com

---

## 📱 PWA Features

- **Installable** — Add to Home Screen on Android, iOS, Windows & macOS.
- **Offline Support** — Loads cached interface without internet.
- **Super-Fast Performance** — Optimized caching and minimal payload.
- **App-Like UI/UX** — Fullscreen, immersive experience.
- **Push-Notification Ready** — Future enhancement.
- **Secure by Default** — HTTPS, service workers, secure headers.
- **Lightweight** — Optimized for low-end devices and Indian network conditions.

---

## 📁 Project Structure


```bash
app.lyfmail.com/
│
├── index.php
├── manifest.php
├── service-worker.js
├── offline.html
├── favicon.ico
├── robots.txt
├── sitemap.xml
├── .htaccess
│
├── css/
│   └── styles.css
│
├── js/
│   └── app.js
│
└── assets/
    ├── logo/
    │   └── logo.png
    ├── icons/
    │   ├── icon-192.png
    │   ├── icon-512.png
    │   └── icon-512-maskable.png
    └── seo/
        ├── og-lyfmail-app.jpg
        ├── twitter-lyfmail-app.jpg
        └── screenshot-lyfmail-app.png
```



---


🔧 Tech Stack
    • PHP (for dynamic manifest + routing).
    • JavaScript (service worker, caching logic, UI functions).
    • HTML/CSS.
    • Web App Manifest (served via PHP).

📦 Installation (For Developers)

1. Clone the Repository

git clone https://github.com/lyfmail-official/lyfmail.git

cd lyfmail

2. No Build Tools Required

This PWA does not require npm, composer, bundlers, or frameworks.

It works on any Linux server with:
    • PHP 7+
    • HTTPS enabled

3. Deploy to Your Server

Upload all files to your hosting:

public_html/

or

your-subdomain/

or

app.domain.com/

4. Ensure HTTPS is Active

PWAs require SSL to install on devices.

5. Register the Service Worker

Ensure this code exists inside <head> of index.php:

<link rel="manifest" href="/manifest.php">

```

<script>
if ("serviceWorker" in navigator) {
    navigator.serviceWorker.register("/service-worker.js");
}
</script>
```

🌐 Deployment

You can deploy the PWA anywhere that supports HTTPS:

* GitHub Pages
* Netlify
* Vercel
* CyberPanel + OpenLiteSpeed
* Any VPS/Shared Hosting

Upload the `build/` or `public/` folder to your server.

📲 How Users Install LYF Mail PWA

1. Visit **[LYF Mail](https://lyfmail.com)** or your subdomain.
2. Browser will show “Add to Home Screen” prompt.
3. Tap Install.
4. LYF Mail becomes an app on the device.

🛡️ Security

* Fully HTTPS compliant.
* CSRF & CORS ready.
* Follows PWA security best practices.
* No sensitive data stored in browser.

🗂️ Roadmap

* Push notifications.
* Offline email drafts.
* Multiple account support.
* Dark mode.
* Performance upgrades.

🤝 Contributing

We welcome contributions!

## 📱 App Preview

![LYF Mail App Preview](assets/seo/screenshot-lyfmail-app.png)


**Maintained by [LYF Mail](https://github.com/lyfmail-official)** · 
Founded by [Ajay Kumar Chaudhary](https://github.com/lyfmail) 
