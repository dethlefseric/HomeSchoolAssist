# Homeschool Assistant - Web App

A Progressive Web App for managing homeschool schedules and household tasks. Works on iPad, iPhone, and any browser!

## 🚀 Super Quick Start

### Easiest Method (2 minutes):

1. Go to https://netlify.com/drop
2. Drag the `HomeschoolAssistantWeb` folder onto the page
3. Wait 10 seconds
4. Open the link you get
5. **Done!** 🎉

### Add to iPad Home Screen:

1. Open in Safari
2. Tap Share button
3. "Add to Home Screen"
4. Now it's an app!

---

## ✨ Features

- 📅 **Daily Schedule** - Plan homeschool lessons and household tasks
- ⭐ **Favorites** - Save templates for recurring activities
- ✅ **Progress Tracking** - See daily completion percentage
- 📆 **Week View** - Overview of the whole week
- 💾 **Offline First** - Works without internet
- 📱 **Install as App** - Add to home screen
- 🖨️ **Print Schedules** - Print your daily plan
- 📤 **Export Data** - Backup to JSON file

---

## 📁 Files

- `index.html` - The complete app (everything in one file!)
- `manifest.json` - PWA configuration
- `sw.js` - Service worker for offline mode
- `SETUP.md` - Detailed setup instructions
- Icons - Create your own at https://favicon.io

---

## 🎨 How It Works

### Today View
- Add tasks with time and duration
- Mark tasks complete with checkbox
- See progress bar
- Filter by type (Homeschool/Household)

### Favorites
- Create reusable templates
- Quick add to any date
- Track usage count

### Schedule
- Week overview
- Task count per day
- Completion percentage

### Settings
- Adjust default durations
- Export/backup data
- Reset if needed

---

## 💡 Pro Tips

**Customize Colors:**
Open `index.html`, find line ~16, change:
```css
--color-primary: #6366f1;  /* Your favorite color! */
```

**Backup Your Data:**
Settings → Export All Data (saves JSON file)

**Print Schedule:**
Menu (⋯) → Print Today's Schedule

**Share with Family:**
Just send them the same link! (Everyone has their own data)

---

## 🛠️ Technical Details

- **Framework**: Vanilla JavaScript (no dependencies!)
- **Storage**: localStorage (browser-based)
- **Offline**: Service Worker + Cache API
- **PWA**: Installable, standalone display
- **Size**: <100KB (super light!)
- **Browser Support**: All modern browsers

---

## 📱 Device Compatibility

Works on:
- ✅ iPad (Safari, Chrome)
- ✅ iPhone (Safari, Chrome)  
- ✅ Android (Chrome, Firefox)
- ✅ Mac/PC (any browser)
- ✅ Kindle Fire (Silk browser)

Best experience: Safari on iOS devices

---

## 🔒 Privacy & Security

- ✅ All data stored locally on your device
- ✅ No external servers
- ✅ No tracking or analytics
- ✅ No account required
- ✅ Works completely offline

Your data never leaves your device!

---

## 🎯 Use Cases

Perfect for:
- Homeschooling families
- Daily routine planning
- Household task management
- Kids' activity scheduling
- Homeschool co-ops
- Multi-child schedules

---

## 🚀 Deployment Options

### Free Hosting (Recommended)

**Netlify Drop** (Easiest)
- Drag folder to https://netlify.com/drop
- Instant deployment
- Custom domain available

**GitHub Pages** (Most Popular)
- Push to GitHub
- Enable Pages in settings
- Free custom domain

**Vercel** (Fast)
- Import from GitHub
- Automatic deployments
- Great performance

### Local Only
- Just open `index.html` in browser
- No internet needed
- Data stays on that computer

---

## 📝 Customization Ideas

Easy to add:
- [ ] More task types (add to type select)
- [ ] Color themes (change CSS variables)
- [ ] Recurring tasks (add recurrence field)
- [ ] Multiple profiles (add profile selector)
- [ ] Custom categories (add category field)
- [ ] Time tracking (add timer)
- [ ] Notifications (use Notification API)
- [ ] Dark mode (add dark theme CSS)

Advanced (requires backend):
- [ ] Cloud sync (Firebase/Supabase)
- [ ] Family sharing (multi-user)
- [ ] Push notifications
- [ ] Email reminders

---

## 🤝 Contributing

Want to improve it? The code is:
- All in one file (easy to understand)
- Well commented
- Standard HTML/CSS/JS
- No build process needed

Just edit `index.html` and refresh!

---

## 📄 License

Free to use and modify for personal or commercial use.

---

## 🆘 Support

Check `SETUP.md` for:
- Detailed setup instructions
- Troubleshooting guide
- Customization tips
- FAQ

---

## 🎉 You're All Set!

1. Upload to Netlify Drop
2. Add to home screen
3. Start planning your homeschool day!

**Questions?** Everything you need is in the SETUP.md file.

Happy Homeschooling! 📚✨
