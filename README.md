# Pamoja — Community Loans App

A modern, offline-first web app for managing community loans and payments. All data is stored locally in your browser—no server needed!

## ✨ What's New in This Version

### Fixed Issues
- ✅ **Persistent Tokens** — User tokens no longer regenerate. They're saved in localStorage and persist across sessions
- ✅ **Modernized UI** — Beautiful gradients, smooth animations, and improved typography
- ✅ **Better UX** — Faster interactions, loading states, and visual feedback
- ✅ **Data Backup** — Export/restore your data as JSON

### Key Features
- 💳 Send and request payments
- 👥 Manage contacts and balances
- 🔐 Secure PIN-based authentication
- 📱 Fully responsive (mobile-first)
- 💾 Automatic localStorage persistence
- 🎨 Modern gradient design with smooth animations
- 📊 Transaction history and balance tracking

## 🚀 Hosting on GitHub Pages (Free!)

### Step 1: Create a GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Name it `pamoja` (or anything you like)
3. Click **Create repository**

### Step 2: Upload the Files

**Option A: Web Upload (Easiest)**
1. Click **Add file** → **Upload files**
2. Drag and drop `index.html` into the browser
3. Click **Commit changes**

**Option B: Git Command Line**
```bash
git clone https://github.com/YOUR_USERNAME/pamoja.git
cd pamoja
cp index.html .
git add index.html
git commit -m "Add Pamoja app"
git push origin main
```

### Step 3: Enable GitHub Pages

1. Go to repository **Settings** → **Pages**
2. Under "Source", select **Branch: main** (or master)
3. Click **Save**
4. Wait 1-2 minutes, then visit: `https://YOUR_USERNAME.github.io/pamoja`

✅ **Your app is now live!** 

## 💡 How It Works

**All data is stored locally in your browser** using `localStorage`. This means:
- ✅ Works completely offline
- ✅ No server needed
- ✅ Privacy is built-in (data never leaves your device)
- ✅ Instant sync across multiple instances

### Storage Structure
```
localStorage['pamoja-state'] = {
  users: [...],           // All user accounts
  transactions: [...],    // Payment history
  requests: [...],        // Payment requests
  currentUser: {...}      // Logged-in user
}
```

## 🔄 Sharing Between Devices

To use the same account on another device:
1. Go to **Profile** → **💾 Backup Data**
2. A JSON file downloads
3. On the other device, go to **Profile** → **📂 Restore Data**
4. Select the downloaded file
5. Done! Your account and all data are restored

## 👥 Multi-User Setup

To test with multiple users on the same device:
1. Open the app in a **new private/incognito window**
2. Create a different account
3. Users can see each other (they're saved globally)
4. Exchange tokens to send/request payments

## 🔐 Security Notes

- PINs are stored locally (not encrypted in this version)
- Tokens are randomly generated, 12-character alphanumeric codes
- For production use, consider adding encryption libraries
- Data persists even after closing the browser

## 📱 Responsive Design

- ✅ Works on mobile, tablet, and desktop
- ✅ Touch-optimized buttons and spacing
- ✅ Smooth animations on all devices
- ✅ Haptic feedback support (browser-dependent)

## 🎨 Customization

### Change Brand Colors
Edit the CSS variables at the top of `index.html`:
```css
:root {
  --gd: #1A3A2A;      /* Dark green */
  --gl: #4A8C63;      /* Light green */
  --amb: #D4821A;     /* Amber */
  --sand: #F5EDD6;    /* Background */
}
```

### Change App Name
Find `Pamoja` in the HTML and replace with your app name.

## 🐛 Troubleshooting

### Data disappeared after refresh
- Check browser console for localStorage errors
- Try exporting and re-importing backup

### App not loading on GitHub Pages
- Verify file is named exactly `index.html`
- Wait 2 minutes after pushing changes
- Hard refresh (Ctrl+Shift+R on Windows, Cmd+Shift+R on Mac)

### Tokens not persisting
- Clear browser cache and localStorage
- Export backup, clear browser data, then restore backup

## 📦 No Dependencies

This is a single HTML file with **zero dependencies**:
- No Node.js
- No build tools
- No CDN dependencies
- Just HTML + CSS + JavaScript

Perfect for offline-first community apps!

## 📄 License

Free to use, modify, and distribute.

## 💬 Support

If you encounter issues:
1. Check browser console (F12 → Console tab)
2. Try clearing localStorage: Open DevTools → Application → LocalStorage → Clear all
3. Test in a different browser

---

**Happy lending!** 🎉

Pamoja = "Together" in Swahili 🇰🇪
