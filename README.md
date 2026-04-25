# 📚 Generic Study Tracker

A **free, customizable study tracker** for any course, subject, or exam. Perfect for students preparing for languages, certifications, tests, or any learning goal.

**No signup. No accounts. No servers. 100% private.**

---

## ✨ Features

### Core Tracking
- ✅ **Track any subject** - English, Biology, Spanish, Math, History, etc.
- ✅ **Customizable topics** - Add your own courses and subtopics
- ✅ **Progress tracking** - Checkboxes for completion + percentage for study depth
- ✅ **Auto-saves** - Never lose progress (saves every change + every 5 seconds)
- ✅ **Full offline** - Works without internet after first load

### Dashboard
- 📊 **Overall Progress Gauge** - Color-coded (Red → Orange → Yellow → Green)
- 📅 **Countdown Timer** - Days remaining until exam/deadline
- ⚠️ **Focus Needed Section** - Shows topics in 1-50% progress range
- 💬 **Inspirational Quotes** - Motivational messages for study sessions
- 📈 **Per-Topic Progress** - Individual progress for each subject

### Productivity
- 📝 **Notes per Topic** - Save formulas, key points, explanations
- 🔐 **Private Notes** - All data stays on your device (never sent anywhere)
- 📱 **Mobile Responsive** - Works perfectly on phone, tablet, desktop
- 🔄 **Memory Save** - Remembers which topics you expanded/collapsed
- 🎯 **Smart Navigation** - Click "Focus" items to jump to them

### Accessibility
- 🌐 **Works Offline** - Full functionality without internet
- 📲 **Installable App** - Add to Android home screen
- 🔌 **No Dependencies** - Pure HTML/CSS/JavaScript (no libraries)
- ⚡ **Fast Loading** - Minimal file size, instant startup
- ♿ **Keyboard Friendly** - Tab through inputs, press Enter to save

---

## 🚀 Quick Start

### Method 1: Web Browser (Fastest)
1. Download `tracker-generic.html`
2. Double-click to open in browser
3. Enter course name and exam date
4. Add your topics
5. Start studying!

### Method 2: Online (Live Version)
Visit: [Your GitHub Pages URL]
- No download needed
- Works on any device
- Bookmarkable

### Method 3: GitHub Pages Deployment
[See Deployment section below]

---

## 📖 How to Use

### Initial Setup (30 seconds)
```
1. Course Name: "English Literature"
2. Exam Date: "2026-05-15"
3. Topic 1: "Shakespeare" with subtopics:
   - Romeo & Juliet
   - Macbeth
   - Hamlet
4. Topic 2: "Victorian Literature"
   - Dickens
   - Bronte Sisters
5. Click "Start Tracking"
```

### Daily Usage
```
✓ Check box when topic is completed
% Enter study progress (0-100)
📝 Click Notes to save key points
📊 Watch dashboard update in real-time
```

### Dashboard Navigation
- **Overall Progress** - Shows combined completion %
- **Days Remaining** - Auto-calculates to your deadline
- **Focus Needed** - Topics between 1-50% (click to jump)
- **Quotes** - New motivational quote each session

---

## 🎯 Feature Breakdown

### Progress Tracking
| Feature | What it Does |
|---------|-------------|
| Checkbox (✓) | Mark topic as complete |
| Percentage (%) | Personal study progress (0-100) |
| Gauge Bar | Visual progress (color-coded) |
| Focus Needed | Topics needing work (1-50%) |

### Color System
```
🔴 0-30%:   Red → Orange (Early stage)
🟡 31-50%:  Orange → Yellow (In progress)
🟢 51-75%:  Yellow → Green (Advanced)
✅ 76-100%: Light Green → Dark Green (Mastered)
```

### Data Persistence
```
Auto-saves on:
✓ Every checkbox click
✓ Every percentage change
✓ Every topic expand/collapse
✓ Every 5 seconds (backup)
✓ Page close
✓ Browser refresh

Restored instantly on:
✓ Page reload
✓ Browser reopening
✓ Device restart (data stays local)
```

---

## 💾 Data & Privacy

### Where Data Goes
- **Stored:** Browser localStorage (your device only)
- **Synced:** Nowhere (100% local)
- **Deleted:** When you clear browser data (user controls this)
- **Backed Up:** Not automatically (you own your data)

### What's Stored
```
✓ Checkboxes (completed topics)
✓ Percentages (study progress)
✓ Expansion states (which topics are open)
✓ Notes (your study notes)
✓ Timestamps (when notes were saved)
```

### What's NOT Stored
```
✗ Your identity
✗ Location data
✗ Browser history
✗ Passwords
✗ Account information
```

### Manual Backup
To backup your data:
1. Open browser DevTools (F12)
2. Console tab
3. Paste: `JSON.stringify(localStorage)`
4. Copy output to text file
5. Keep safe

---

## 📱 Installation

### As Android App
1. Open in Chrome/Firefox on Android
2. Menu (⋮) → "Install app" or "Add to Home Screen"
3. App appears on home screen
4. Tap to open anytime
5. Works offline completely

### As iOS Web App
1. Open Safari on iPhone
2. Menu → "Add to Home Screen"
3. App appears on home screen
4. Works like native app
5. Offline support limited (iOS 11.3+)

### On Computer
- Chrome/Firefox/Safari/Edge
- No installation needed
- Just open HTML file
- Or use online version

---

## 🔧 Customization

### Change Colors
Edit CSS variables in `tracker-generic.html`:
```css
:root {
    --primary: #06d6a0;  /* Main color */
    --bg-gradient: linear-gradient(...);  /* Background */
}
```

### Add More Quotes
Add to `quotes` array in script:
```javascript
const quotes = [
    "Your custom quote here",
    "Another motivational message"
];
```

### Modify Gauge Colors
Edit in `updateProgress()` function:
```javascript
if (overallPercent <= 30) {
    color = 'linear-gradient(...)';  // Change red color
}
```

---

## 🌐 Deployment

### Free Hosting Options

#### Option 1: Netlify (Easiest)
```
1. Go to netlify.com
2. Click "Deploy"
3. Drag and drop your files
4. Get live URL instantly
5. Auto-updates when you change files
```

#### Option 2: Vercel
```
1. Go to vercel.com
2. Import from GitHub
3. Deploy (automatic)
4. Get live URL
5. SSL/HTTPS included
```

#### Option 3: GitHub Pages
```
1. Upload files to GitHub repo
2. Settings → Pages
3. Enable from main branch
4. URL: yourusername.github.io/study-tracker
5. Free, built-in
```

#### Option 4: Your Own Server
```
1. Upload files via FTP
2. Enable HTTPS
3. Access via your domain
4. Full control
```

---

## 📋 File Structure

```
study-tracker/
├── tracker-generic.html          # Main app (only file needed!)
├── manifest.json                 # PWA config (for install)
├── service-worker.js             # Offline support
├── offline.html                  # Offline fallback
├── README.md                     # This file
└── GITHUB_SETUP.md              # GitHub deployment guide
```

### Minimum Files Needed
- `tracker-generic.html` (everything in one file)

### Recommended Files (Full Features)
- All 4 files above (offline + installable)

---

## 🛠 Technical Details

### Browser Requirements
- **Modern browsers:** Chrome, Firefox, Safari, Edge
- **Mobile:** iOS 10+, Android 4.4+
- **Offline:** Service Worker support (most devices)
- **Storage:** localStorage (5-10MB available)

### Technologies Used
```
HTML5 - Structure
CSS3 - Styling (flexbox, gradients)
JavaScript (Vanilla) - No libraries
Service Workers - Offline caching
localStorage - Data persistence
```

### Performance
- **File size:** ~50KB (HTML + CSS + JS)
- **Load time:** <1 second
- **Storage per tracker:** ~10-50KB
- **Compatibility:** All modern browsers

---

## 🐛 Troubleshooting

### Data Not Saving
```
✓ Check if localStorage is enabled
✓ Disable private/incognito mode
✓ Clear browser cache
✓ Try different browser
✓ Check available storage
```

### App Won't Load
```
✓ Refresh page (F5 or Ctrl+R)
✓ Hard refresh (Ctrl+Shift+R)
✓ Clear browser cache
✓ Check internet connection
✓ Try different browser
```

### Offline Not Working
```
✓ Load page online first (caches files)
✓ Service Worker needs time to activate
✓ Check browser console for errors
✓ iOS has limited offline support
```

### Lost Progress
```
✓ Check if you cleared browser data
✓ Check different browser
✓ Data deleted on localStorage clear
✓ No cloud backup (local only)
✓ Restore from backup file if saved
```

---

## 🎓 Use Cases

### Students
- Prepare for exams (SAT, GRE, MCAT, etc.)
- Learn languages (Spanish, French, German, etc.)
- Study textbook chapters
- Track certification prep

### Teachers
- Assign tracking to students
- Monitor class progress
- Track curriculum coverage
- Assessment tracking

### Professionals
- Skill development tracking
- Certification prep (IT, Finance, etc.)
- Knowledge management
- Continuous learning

### Personal Development
- New skill learning
- Hobby progress tracking
- Reading goals
- Any learning objective

---

## 🚦 Roadmap

### Coming Soon
- [ ] Dark mode
- [ ] Custom colors per topic
- [ ] Export progress as PDF
- [ ] Cloud backup option
- [ ] Multi-device sync
- [ ] Collaborative tracking
- [ ] Habit stacking
- [ ] Study streak counter

### User Requested
- [ ] Time tracking per topic
- [ ] Spaced repetition reminders
- [ ] Leaderboard/competition mode
- [ ] Mobile app versions

---

## 💡 Tips & Tricks

### Best Practices
```
✓ Set realistic deadlines
✓ Use percentages for depth, checkboxes for completion
✓ Review "Focus Needed" daily
✓ Update notes while studying (not after)
✓ Check progress weekly
✓ Adjust topics based on difficulty
```

### Study Hacks
```
✓ Set percentage to see what needs work
✓ Click "Focus" items to jump directly
✓ Use notes for quick formulas/facts
✓ Check dashboard for motivation
✓ Set harder deadlines for buffer time
```

### For Teachers
```
✓ Share tracker with class
✓ Have students report percentages
✓ Use Focus Needed to identify gaps
✓ Customize for each unit
✓ Print progress for grading
```

---

## 🤝 Contributing

### Found a Bug?
1. Open an issue on GitHub
2. Describe the problem
3. Include browser/device info
4. Provide steps to reproduce

### Have a Feature Idea?
1. Open an issue with tag: `enhancement`
2. Describe what you want
3. Explain why it's useful
4. Vote on existing ideas

### Want to Contribute Code?
1. Fork the repository
2. Create a branch: `git checkout -b feature/my-feature`
3. Make changes
4. Submit pull request
5. We'll review and merge!

---

## 📄 License

MIT License - Use freely for any purpose

### You Can:
- ✅ Use commercially
- ✅ Modify the code
- ✅ Distribute/share
- ✅ Use privately
- ✅ Sublicense

### You Must:
- Include license notice
- State changes made
- That's it!

---

## 🙏 Credits

Built for students, by students.

Special thanks to everyone who:
- Tested the tracker
- Provided feedback
- Suggested features
- Shared with friends

---

## 📞 Support

### Questions?
- Open an issue on GitHub
- Check existing issues for answers
- Check FAQ section below

### Bugs?
- Describe what happened
- Include browser info
- Steps to reproduce
- Screenshots if possible

### Feature Requests?
- Describe the feature
- Why you need it
- How you'd use it
- Upvote if others suggest same

---

## ❓ FAQ

### Q: Is my data safe?
**A:** Yes! All data stays on your device. Never sent to servers. No accounts needed.

### Q: Can I export my data?
**A:** Backup manually via console. Cloud export coming soon.

### Q: Works offline?
**A:** Yes! After first load, works 100% offline.

### Q: Can I use for multiple courses?
**A:** Yes! Create new browser tab or multiple trackers.

### Q: Is it really free?
**A:** Yes, forever. MIT licensed.

### Q: Mobile friendly?
**A:** Perfect on phones, tablets, and desktop.

### Q: Installable as app?
**A:** Yes! Android and iOS (limited).

### Q: Can I share with others?
**A:** Share the link. Everyone gets their own data.

### Q: Will it work in 5 years?
**A:** As long as browsers support localStorage and Service Workers.

### Q: Can I modify it?
**A:** Yes! MIT license allows modifications.

### Q: Is there an API?
**A:** Data is in localStorage (JSON format). Extract and use as needed.

---

## 🎯 Getting Started Right Now

1. **Download:** Get `tracker-generic.html`
2. **Open:** Double-click to start
3. **Setup:** Add your course (30 seconds)
4. **Study:** Start tracking progress
5. **Succeed:** Ace your exam!

---

## 🌟 If You Like This

- ⭐ Star on GitHub
- 📢 Share with friends
- 🐛 Report bugs
- 💡 Suggest features
- 🔗 Link in your community

---

## 📊 Status

✅ Fully functional  
✅ Production ready  
✅ Mobile optimized  
✅ Offline capable  
✅ Privacy focused  
✅ Actively maintained  

---

**Made with ❤️ for students everywhere**

*Last Updated: April 2026*

---

### Quick Links
- [GitHub Repository](#)
- [Live Demo](#)
- [GitHub Setup Guide](./GITHUB_SETUP.md)
- [Original MELE Tracker](https://github.com/yourusername/mele-tracker)

---

**Happy studying! 📚💪**
