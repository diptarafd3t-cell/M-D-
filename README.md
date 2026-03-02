# 🎵 Music.D — Premium YouTube Interface

A cinematic **Glassmorphism** single-page application for an immersive, ad-free viewing experience.

## ✨ Features
* **Ad-Free UI:** Uses `modestbranding` and `iv_load_policy` parameters to strip YouTube site clutter.
* **Secure Access:** Integrated login overlay to protect the stream.
* **Smart URL Parsing:** Robust regex engine supports Desktop, Mobile, and Shorts links.

## 🧪 Technical Logic
The application identifies video IDs using this pattern:
```javascript
const regex = /(?:youtube\.com\/(?:[^\/]+\/.+\/|(?:v|e(?:mbed)?|shorts)\/|.*[?&]v=)|youtu\.be\/)([^"&?\/\s]{11})/;
