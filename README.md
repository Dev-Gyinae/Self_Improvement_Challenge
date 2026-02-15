# 🐔 90-Day Chicken Army Challenge

A gamified habit tracker that transforms your daily tasks into a growing flock of champion chickens. Watch 15 unique colored chickens evolve from eggs to champions as you build consistency over 90 days.

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Maintenance](https://img.shields.io/badge/maintained-yes-brightgreen.svg)

## 🎯 Overview

The Chicken Army Challenge is a visual habit tracking system designed for personal growth and accountability. Each of your 15 habits is represented by a uniquely colored chicken that progressively evolves through 6 distinct growth stages based on your consistency.

### Why Chickens?

Unlike traditional habit trackers, the Chicken Army uses a unified evolution system where every chicken follows the same growth path, making progress visually intuitive and satisfying to watch. The progressive nature (egg → hatching → baby → juvenile → adult → champion) creates a powerful visual metaphor for personal growth.

## ✨ Features

### Core Functionality
- **15 Unique Chickens**: Each habit represented by a distinctly colored chicken with its own personality
- **6 Growth Stages**: Universal evolution system from egg (0%) to champion (80%+)
- **Real-time Progress**: Visual progress bars and percentage tracking
- **Streak Tracking**: Current and best streak counters for each habit
- **30-Day Calendar**: Visual heat map of completions for the last month
- **Overall Statistics**: Aggregate view of your entire journey

### Data Management
- **Auto-Save**: Progress automatically saved to browser localStorage every minute
- **Backup System**: Export/import your complete progress as JSON files
- **Weekly Reports**: Generate text reports of your progress
- **No Server Required**: Runs entirely in your browser - perfect for offline use

### User Experience
- **Glassmorphism Design**: Modern frosted-glass aesthetic with depth and shadows
- **Smooth Animations**: Stage-specific animations (wobble, shake, bounce, hop, strut, pulse)
- **Responsive Layout**: Works on desktop, tablet, and mobile
- **Dark Theme**: Easy on the eyes for extended use
- **Toast Notifications**: Satisfying feedback for all actions
- **Keyboard Shortcuts**: ESC to close modals

## 🐣 Evolution System

Each chicken evolves through 6 stages based on completion rate:

| Stage | Emoji | Completion Rate | Animation | Meaning |
|-------|-------|----------------|-----------|---------|
| **Egg** | 🥚 | 0-10% | Gentle wobble | Just starting out |
| **Hatching** | 🐣 | 10-20% | Cracking shake | Breaking through resistance |
| **Baby** | 🐤 | 20-40% | Cute bounce | Building momentum |
| **Juvenile** | 🐥 | 40-60% | Energetic hop | Consistent progress |
| **Adult** | 🐔 | 60-80% | Confident strut | Strong habits formed |
| **Champion** | 🐓 | 80%+ | Power pulse | Mastery achieved |

**Example**: If you're on Day 30 and have completed a task 24 times, your chicken is at 80% (24/30), making it a Champion! 🐓

## 🎨 The 15 Chickens

Each task has a unique colored chicken with its own theme:

1. **🏃 Jogging** - Red Runner (8000 steps daily)
2. **💪 P90X** - Purple Power (Full workout routine)
3. **🧘 Meditation** - Blue Zen (Daily mindfulness practice)
4. **📖 Sermon** - White Divine (Spiritual study/listening)
5. **📚 Reading** - Brown Scholar (Daily reading)
6. **⚙️ DevOps** - Gray Tech (Technical practice/learning)
7. **🐙 Git & OSS** - Green Collab (Version control & open source)
8. **💼 Job Search** - Black Professional (Applications & networking)
9. **📊 AdHive Business** - Gold Entrepreneur (Business development)
10. **♟️ Chess** - Checkered Strategist (Practice & puzzles)
11. **🇩🇪 German** - Yellow-Red Polyglot (Language practice)
12. **🔥 Bodyweight Circuit** - Orange Fire (50 reps × 6 exercises)
13. **🧠 Key Knowledge** - Cyan Brain (Review & study)
14. **⚡ Semen Retention** - Electric Yellow (NoFap discipline)
15. **🧊 Straight Edge** - Ice Crystal (Substance-free lifestyle)

## 🚀 Getting Started

### Installation

1. **Download the file**:
   ```bash
   git clone https://github.com/yourusername/chicken-army-challenge.git
   cd chicken-army-challenge
   ```

2. **Open in browser**:
   - Simply double-click `chicken-army-tracker.html`
   - Or right-click → Open with → Your preferred browser

That's it! No dependencies, no build process, no server required.

### First Steps

1. **Day 1**: All chickens start as eggs 🥚
2. **Mark completions**: Click "Complete Today" for each task you finish
3. **Watch them grow**: Chickens evolve based on your consistency rate
4. **Track progress**: Click "📊 Details" on any chicken to see detailed stats
5. **Backup regularly**: Use "💾 Save Backup" to protect your progress

## 📊 How to Use

### Daily Workflow

1. Open the tracker in your browser
2. Complete your daily habits
3. Mark each completed task by clicking "Complete Today"
4. Watch the celebration animation! 🎉
5. Check your overall consistency score

### Backup Your Progress

**To Save**:
1. Click "💾 Save Backup" (top right)
2. Downloads a JSON file with all your data
3. Store it safely (cloud storage recommended)

**To Restore**:
1. Click "📂 Restore Backup"
2. Select your backup JSON file
3. All progress instantly restored

### Weekly Reports

Generate a text report of your progress:
1. Click "📊 Weekly Report"
2. Opens a text file showing:
   - Overall stats
   - Each chicken's progress
   - Streaks and completion rates
   - Current stage of each habit

## 💾 Data Storage

### Local Storage
- All data stored in browser's localStorage
- Persists between sessions
- Automatically saved every minute
- No data sent to any server

### Backup Files
- JSON format (human-readable)
- Contains all completions, dates, and metadata
- Can be manually edited if needed
- Import/export across devices

### Storage Structure
```json
{
  "startDate": "2025-01-01T00:00:00.000Z",
  "lastBackup": "2025-01-15T12:30:00.000Z",
  "tasks": {
    "jogging": {
      "completions": {
        "2025-01-01": true,
        "2025-01-02": true
      }
    }
  },
  "version": "1.0"
}
```

## 🔧 Customization

Want to adapt this for your own habits? Easy! Just edit the `CONFIG.tasks` object in the HTML file:

```javascript
const CONFIG = {
    duration: 90,  // Change challenge duration
    tasks: {
        yourhabit: {
            name: "🎯 Your Habit",
            category: "Your Category",
            subtasks: "Your description",
            chickenColor: "Your Color",
            description: "Your chicken's personality"
        }
    }
};
```

## 📱 Browser Compatibility

- ✅ Chrome/Edge (90+)
- ✅ Firefox (85+)
- ✅ Safari (14+)
- ✅ Opera (75+)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

**Minimum Requirements**: 
- JavaScript enabled
- localStorage support
- CSS3 animations support

## 🎯 Tips for Success

### Building Consistency
1. **Start small**: Don't try to complete all 15 tasks on Day 1
2. **Focus on streaks**: Even 1-day streaks are wins
3. **Use the 2-day rule**: Never miss twice in a row
4. **Celebrate eggs**: Even starting is progress
5. **Backup weekly**: Protect your hard work

### Motivation Strategies
- **Visual goal**: Watch for the Champion stage (🐓)
- **Compete with yourself**: Try to beat your best streaks
- **Weekly reviews**: Generate reports to see trends
- **Share progress**: Export reports to accountability partners
- **Celebrate milestones**: Day 30, 60, 90

### Common Pitfalls
- ❌ Being too harsh on missed days → ✅ Focus on getting back on track
- ❌ Aiming for 100% instantly → ✅ Gradual improvement is sustainable
- ❌ Not backing up → ✅ Set a weekly backup reminder
- ❌ All-or-nothing thinking → ✅ Partial completion > no completion

## 🤝 Contributing

This is a personal project, but suggestions are welcome!

### Ways to Contribute
- 🐛 Report bugs via Issues
- 💡 Suggest new features
- 🎨 Propose design improvements
- 📖 Improve documentation
- 🔀 Submit pull requests

### Development
The project is a single HTML file with embedded CSS and JavaScript. No build tools required!

```bash
# Fork the repo
# Make your changes
# Test in multiple browsers
# Submit a pull request
```

## 📄 License

MIT License - Feel free to use, modify, and distribute!

```
Copyright (c) 2025

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
```

## 🙏 Acknowledgments

- Inspired by habit tracking methodologies from James Clear's "Atomic Habits"
- Evolution system concept from gamification principles
- Emoji chickens courtesy of Unicode Consortium 🐔

## 📞 Support

Having issues? Want to share your success?

- 📧 Email: dev.gyinae@gmail.com
- 💬 Discussions: GitHub Discussions tab

## 🗺️ Roadmap

Future enhancements being considered:

- [ ] Sound effects toggle (optional audio feedback)
- [ ] Export progress as images/infographics
- [ ] Social sharing features
- [ ] Multiple challenge modes (30-day, 60-day, custom)
- [ ] Habit categories grouping
- [ ] Dark/light theme toggle
- [ ] Custom chicken colors
- [ ] Achievement badges system
- [ ] Comparison with previous challenges
- [ ] CSV export for data analysis

## 📈 Stats

Track your usage:
- **Day 1**: All eggs 🥚
- **Day 30**: First evolutions appear
- **Day 60**: Champions start emerging 🐓
- **Day 90**: Complete flock of champions!

---

**Remember**: Every champion chicken started as an egg. Your journey begins today! 🥚➡️🐓

*Made with ❤️ and lots of 🐔 emojis*
