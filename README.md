**[LYF Mail](https://lyfmail.com)** – PWA (Progressive Web App)

The official open-source Progressive Web App for LYF Mail, designed to deliver a fast, reliable, mobile-first email experience across all devices.

This PWA allows users to access LYF Mail directly from their home screen, enjoy offline capabilities, near-instant loading, and a clean, app-like interface without needing to install anything from app stores.

🚀 Features

* Installable App – Users can install LYF Mail on Android, iOS, Windows & macOS.
* Offline Support – Loads cached interface even without internet.
* Super-Fast Performance using optimized caching.
* App-Like UI/UX with fullscreen experience.
* Push-Notification Ready (future enhancement).
* Secure by Default – HTTPS, service workers, manifest configuration.
* Lightweight and optimized for low-end devices.

📁 Project Structure

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


🚀 Features
    • Installable on any device (A2HS – Add to Home Screen)
    • Offline Support with service-worker.js
    • Dynamic Manifest via manifest.php
    • Custom Offline Page (offline.html)
    • SEO-Optimized with OG + Twitter images
    • Fast Loading with optimized CSS/JS
    • HTTPS + Secure Headers
    • Full App-like UI using index.php fullscreen mode

🔧 Tech Stack
    • PHP (for dynamic manifest + routing)
    • JavaScript (service worker, caching logic, UI functions)
    • HTML/CSS
    • Web App Manifest (served via PHP)

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

<script>
if ("serviceWorker" in navigator) {
    navigator.serviceWorker.register("/service-worker.js");
}
</script>

🌐 Deployment

You can deploy the PWA anywhere that supports HTTPS:

* GitHub Pages
* Netlify
* Vercel
* CyberPanel + OpenLiteSpeed
* Any VPS/Shared Hosting

Upload the `build/` or `public/` folder to your server.

📲 How Users Install LYF Mail PWA

1. Visit your domain (main site or subdomain).
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
