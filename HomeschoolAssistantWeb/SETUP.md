# Homeschool Assistant - Web App Setup Guide

## 🎉 Welcome! This is MUCH Easier Than the iOS Version

Since you're using an iPad, this web app version is perfect. It works on:
- ✅ iPad (Safari, Chrome)
- ✅ iPhone (Safari, Chrome)
- ✅ Any computer browser
- ✅ Android devices

**No Mac required! No Xcode needed!**

---

## Quick Start (5-10 Minutes)

### Option 1: Use Online (Easiest - 2 minutes)

If you just want to use it right now:

1. **Upload to a free hosting service**
   - Go to https://netlify.com/drop
   - Drag the entire `HomeschoolAssistantWeb` folder onto the page
   - Wait 10 seconds
   - You'll get a link like: `https://your-app-name.netlify.app`
   - **That's it! Open that link on your iPad**

2. **Add to your iPad home screen**
   - Open the link in Safari on your iPad
   - Tap the Share button (square with arrow)
   - Scroll down and tap "Add to Home Screen"
   - Tap "Add"
   - Now it looks and works like a real app! 📱

### Option 2: Run Locally (More Control - 5 minutes)

If you want to test it on your computer first:

**On Mac/Linux:**
```bash
cd HomeschoolAssistantWeb
python3 -m http.server 8000
```

**On Windows:**
```bash
cd HomeschoolAssistantWeb
python -m http.server 8000
```

Then open: http://localhost:8000

---

## How to Use the App

### 📅 **Today Tab**
1. **Add a Task**
   - Tap the blue "+" button
   - Fill in: Title, Type (Homeschool/Household), Time, Duration
   - Tap "Save"

2. **Complete a Task**
   - Tap the circle checkbox next to any task
   - It turns green ✓
   - Progress bar updates automatically

3. **View Task Details**
   - Tap any task card
   - See all details
   - Edit or delete the task

4. **Filter Tasks**
   - Tap "All", "Homeschool", or "Household" buttons
   - View only tasks of that type

### ⭐ **Favorites Tab**
1. **Create a Favorite Template**
   - Tap the "+" button
   - Example: "Math Lesson - 30 min"
   - Save it

2. **Quick Add from Favorite**
   - Tap the "+" icon on any favorite
   - Choose date and time
   - Instantly creates a task!

3. **Edit/Delete Favorites**
   - Tap the pencil icon to edit
   - Tap the trash icon to delete

### 📆 **Schedule Tab**
- View the whole week at a glance
- See how many tasks each day
- See completion percentage per day

### ⚙️ **Settings Tab**
- Adjust default durations
- Export your data (backup)
- Reset all data if needed

---

## Features Included

✅ **Offline-First** - Works without internet (after first load)
✅ **Add to Home Screen** - Looks like a real app
✅ **Dual Schedule** - Homeschool + Household tasks
✅ **Quick Picks** - Favorite templates
✅ **Progress Tracking** - See daily completion %
✅ **Week View** - See the whole week
✅ **Print Support** - Print schedules
✅ **Data Export** - Backup to JSON file
✅ **Responsive** - Works on any screen size

---

## Installation Methods Compared

### Netlify Drop (Recommended for You)
- ⏱️ **Time**: 2 minutes
- 💰 **Cost**: Free
- 🔧 **Difficulty**: Drag and drop
- 📱 **Works on iPad**: Yes
- 🌐 **Need Internet**: First time only

**Steps:**
1. Go to https://netlify.com/drop
2. Drag the folder
3. Get your link
4. Done!

### GitHub Pages (Free, More Permanent)
- ⏱️ **Time**: 10 minutes
- 💰 **Cost**: Free
- 🔧 **Difficulty**: Easy (if you know GitHub)
- 📱 **Works on iPad**: Yes

**Steps:**
1. Create GitHub account (github.com)
2. Create new repository
3. Upload files
4. Enable GitHub Pages in settings
5. Get link: `https://yourusername.github.io/homeschool-assistant`

### Local File (No Internet Needed)
- ⏱️ **Time**: 1 minute
- 💰 **Cost**: Free
- 🔧 **Difficulty**: Super easy
- 📱 **Works on iPad**: Yes, but harder to set up

**Steps:**
1. Download the files to your iPad
2. Open `index.html` in Safari
3. Works, but you'll lose data if you clear browser

---

## Adding to iPad Home Screen

This makes it feel like a native app!

1. **Open in Safari** (must be Safari, not Chrome)
2. **Tap the Share button** (square with arrow up)
3. **Scroll down** and tap "Add to Home Screen"
4. **Choose a name** (or keep "Homeschool Assistant")
5. **Tap "Add"**

Now you have an app icon on your home screen! When you open it:
- ✅ No browser bars (looks like a real app)
- ✅ Full screen
- ✅ Faster loading
- ✅ Works offline

---

## Customization

### Change Colors
Open `index.html` and find this section (around line 16):

```css
:root {
    --color-primary: #6366f1;        /* Main blue - change this! */
    --color-homeschool: #3b82f6;     /* Homeschool badge color */
    --color-household: #10b981;      /* Household badge color */
}
```

**Popular color schemes:**
- Purple theme: `#9333ea`
- Pink theme: `#ec4899`
- Orange theme: `#f97316`
- Teal theme: `#14b8a6`

### Add App Icons
1. Create icons at https://favicon.io/favicon-generator/
2. Download the 192x192 and 512x512 versions
3. Rename them to `icon-192.png` and `icon-512.png`
4. Put them in the same folder as `index.html`

---

## Data Storage

**Where is my data saved?**
- All data is stored in your browser's localStorage
- It stays on your device (private and secure)
- Survives app restarts
- Syncs if you use the same browser/account

**Will I lose my data?**
- ❌ NO if you just close the app
- ❌ NO if you restart your device
- ⚠️ YES if you clear browser data/cache
- ⚠️ YES if you use a different browser

**How to backup:**
1. Go to Settings tab
2. Tap "Export All Data"
3. Saves a JSON file you can re-import later

---

## Troubleshooting

### App not saving data
- Make sure you're using Safari (best support)
- Don't use Private/Incognito mode
- Check if you have enough storage on device

### Can't add to home screen
- Must use Safari browser (not Chrome)
- Make sure you're on the actual website, not a local file

### App looks weird on iPad
- Refresh the page
- Clear cache and reload
- Try landscape and portrait mode

### Want to share with family
- Everyone needs the same link
- Data is NOT shared (each person has their own)
- To share data, use Export/Import feature

---

## Going Further

### Want to Sync Between Devices?
You'll need to add a backend service like:
- Firebase (free tier available)
- Supabase (free tier available)
- Your own server

I can help you add this if needed!

### Want More Features?
The code is easy to modify:
- All in one file (`index.html`)
- Clear comments throughout
- Standard HTML/CSS/JavaScript
- No build tools needed

---

## File Structure

```
HomeschoolAssistantWeb/
├── index.html          ← The entire app (open this!)
├── manifest.json       ← PWA configuration
├── sw.js              ← Service worker (offline mode)
├── icon-192.png       ← App icon (you create this)
├── icon-512.png       ← App icon (you create this)
└── SETUP.md           ← This file
```

**That's literally it!** One HTML file has everything.

---

## Quick Test Checklist

After setting up, test these:

- [ ] Open the app
- [ ] Create a task
- [ ] Mark task complete
- [ ] Create a favorite
- [ ] Quick add from favorite
- [ ] View schedule tab
- [ ] Change settings
- [ ] Export data
- [ ] Close and reopen (data should persist!)
- [ ] Add to home screen
- [ ] Open from home screen icon

---

## Need Help?

**Common Questions:**

**Q: Can I use this on iPhone?**
A: Yes! Same setup process.

**Q: Will it work offline?**
A: Yes, after first load. It caches everything.

**Q: Can I print schedules?**
A: Yes! Use the menu button → Print.

**Q: How do I update the app?**
A: Just upload new files to same location, refresh page.

**Q: Can I change the name?**
A: Yes! Edit `manifest.json` and change "name" field.

---

## Comparison: Web App vs iOS App

| Feature | Web App (This One) | iOS App (Previous) |
|---------|-------------------|-------------------|
| Works on iPad | ✅ Yes | ❌ Need Mac to build |
| Setup Time | 5 minutes | 30+ minutes |
| Looks Native | ⚠️ Close | ✅ Perfect |
| Offline | ✅ Yes | ✅ Yes |
| App Store | ❌ No | ✅ Possible |
| Updates | Easy (just refresh) | Need rebuild |
| Sharing | Easy (send link) | Hard (TestFlight) |

**Bottom Line:** For your situation (iPad only), the web app is PERFECT! 🎉

---

**Ready to start? Just drag the folder to Netlify Drop and you're done!**

Questions? Everything you need is in this one HTML file. Good luck! 🚀
