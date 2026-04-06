# 🌐 Lingua AI – Universal Translator

## Files in this package
```
translator-pwa/
├── index.html      ← Main app
├── manifest.json   ← PWA config
├── sw.js           ← Service worker (offline support)
└── icons/          ← App icons (all sizes)
```

---

## 🚀 Option 1: Deploy PWA (Free, 5 minutes)

### Step 1 – Upload to Netlify (easiest)
1. Go to **https://netlify.com** → Sign up free
2. Drag & drop the entire `translator-pwa` folder onto the Netlify dashboard
3. You'll get a live URL like: `https://lingua-ai-abc123.netlify.app`

### Step 2 – Install on Android
1. Open Chrome on your Android phone
2. Visit your Netlify URL
3. Tap the **⋮ menu → "Add to Home screen"**
4. Tap **Install** — done! 🎉

### Step 3 – Install on iPhone
1. Open Safari on iPhone
2. Visit your Netlify URL
3. Tap **Share → Add to Home Screen**
4. Tap **Add** — done! 🎉

---

## 📱 Option 2: Use the APK (Android only)

The `LinguaAI.apk` file is included alongside this folder.

### Install APK on Android:
1. Copy `LinguaAI.apk` to your Android phone (via USB, email, or Google Drive)
2. On phone: **Settings → Security → Enable "Unknown Sources"**
   (on Android 8+: Settings → Apps → Special access → Install unknown apps → Files → Allow)
3. Open your Files app, tap `LinguaAI.apk`
4. Tap **Install**
5. Open **Lingua AI** from your app drawer! 🎉

> ⚠️ Note: The APK requires internet to translate (it calls the Claude AI API).

---

## 🔑 API Key

The app uses the Claude AI API. You need to add your own API key:

1. Get a free API key at: **https://console.anthropic.com**
2. Open `index.html` in a text editor
3. Find this line: `headers: { 'Content-Type': 'application/json' }`
4. Add your key: `'x-api-key': 'YOUR_KEY_HERE', 'anthropic-version': '2023-06-01'`

---

## ✅ Features
- 100+ languages supported
- Auto-detect language
- Offline app shell (loads without internet)
- Copy translation with one tap
- Keyboard shortcut: Ctrl/Cmd + Enter
- Works on Android, iPhone, and desktop
