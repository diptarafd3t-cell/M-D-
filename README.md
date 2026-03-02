# 🎵 Music.D — Premium YouTube Interface

A cinematic **Glassmorphism** single-page application for an immersive, ad-free viewing experience.

## ✨ Features
* **Ad-Free UI:** Uses `modestbranding` and `iv_load_policy` parameters to strip YouTube site clutter.
* **Secure Access:** Integrated login overlay to protect the stream.
* **Smart URL Parsing:** Robust regex engine supports Desktop, Mobile, and Shorts links.

## 🧪 Technical Logic
The application identifies video IDs using this pattern:
```javascript
const regex = /(?:youtube\.com\
// Source - https://stackoverflow.com/q/6903823

// Posted by Stanley, modified by community. See post 'Timeline' for change history

// Retrieved 2026-03-02, License - CC BY-SA 3.0



var url = "http://www.youtube.com/sandalsResorts#p/c/54B8C800269D7C1B/0/FJUvudQsKCM";
//var url = "http://www.youtube.com/user/Scobleizer#p/u/1/1p3vcRhsYGo";
//var url = "http://youtu.be/NLqAF9hrVbY";
//var url = "http://www.youtube.com/embed/NLqAF9hrVbY";
//var url = "https://www.youtube.com/embed/NLqAF9hrVbY";
//var url = "http://www.youtube.com/v/NLqAF9hrVbY?fs=1&hl=en_US";
//var url = "http://www.youtube.com/watch?v=NLqAF9hrVbY";
//var url = "http://www.youtube.com/user/Scobleizer#p/u/1/1p3vcRhsYGo";
//var url = "http://www.youtube.com/ytscreeningroom?v=NRHVzbJVx8I";
//var url = "http://www.youtube.com/user/Scobleizer#p/u/1/1p3vcRhsYGo";
//var url = "http://www.youtube.com/watch?v=JYArUl0TzhA&feature=featured";

var videoID = url.match(/(?:youtu\.be\/|youtube\.com(?:\/embed\/|\/v\/|\/watch\?v=|\/user\/\S+|\/ytscreeningroom\?v=))([\w\-]{10,12})\b/)[1];
alert(videoID);
