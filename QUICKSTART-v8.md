# Task Duel v8.0 - QUICK START GUIDE

## 🚀 30-SECOND SETUP

### Step 1: Download the App
- Download: `task-duel-v8.0.html` (attached file)

### Step 2: Deploy to GitHub Pages (2 minutes)
```
1. Create GitHub account (if needed) → github.com
2. Create new public repo: "task-duel-v8"
3. Upload task-duel-v8.0.html as "index.html"
4. Settings → Pages → Deploy from main branch
5. Copy your URL: https://USERNAME.github.io/task-duel-v8
```

### Step 3: Install on iPhone (3 minutes)
```
1. iPhone Safari → Paste your GitHub Pages URL
2. Bottom Share icon → "Add to Home Screen"
3. Name: "Task Duel"
4. Tap "Add"
5. Done! Native app on home screen
```

### Step 4: First Login
```
Password: "ChangeMeToYourPassword2025"
→ Change this immediately in Settings!
```

---

## 📱 WHAT YOU GET

| Feature | What It Does | Time |
|---------|------------|------|
| **Dashboard** | Overview of progress | Always visible |
| **Duel Arena** | Compare 2 options, rank by preference | 10-15 min |
| **Forge** | Quiz yourself to generate items | 5-10 min |
| **Gap Bridge** | Map current self → ideal self | 5 min |
| **Neural Forge** | Daily transformation rituals | 5 min |
| **Analytics** | Track progress + export data | 2 min |
| **Settings** | Customize + backup data | As needed |

---

## ⚡ YOUR FIRST 10 MINUTES

### Minute 1-2: Onboarding
- Open app on iPhone
- Enter password
- See Dashboard

### Minute 3-5: Try Forge
- Tap "🎯 Forge" tab
- Click "💪 Physical"
- Answer 3 quick questions
- System generates items

### Minute 6-8: Start Dueling
- Tap "⚔️ Duel" tab
- Click "📝 Tasks"
- Compare 2 items
- Pick which you prefer
- Repeat 10 times

### Minute 9-10: Check Analytics
- Tap "📈 Analytics"
- See your stats
- Tap "JSON" to export

---

## 🎯 DAILY ROUTINE

### Morning (5 minutes)
```
1. Tap "🧠 Neural" tab
2. "🎬 Visualization" → Start → Wait 90s
3. Log 3 wins in "📝 Micro-Evidence"
4. Tap "✓ Completed Today"
→ Done! Continue with your day
```

### Anytime (10 minutes)
```
1. "🎯 Forge" tab
2. Pick a quiz (Physical/Career/Dating/etc)
3. Answer questions
4. System creates preset
5. "⚔️ Duel" tab
6. Compare items
→ Preference data logged
```

### Evening (Optional)
```
1. "📈 Analytics" tab
2. Check phase % progress
3. Export if backing up
```

---

## 🔑 KEY CONCEPTS

### What is "Dueling"?
You see 2 options. Pick which one matters MORE to you.
- Left card vs Right card
- Pick one (don't overthink)
- System learns your preferences
- Over 100 duels = clear pattern emerges

### What is "Forge"?
You answer questions about what you want. System turns answers into duel items.
- "What body goals?" → "Six-pack abs", "White teeth"
- "Career preferences?" → "Solo work", "Flexible hours"
- Creates database of YOUR priorities

### What is "Gap Bridge"?
Connect who you are now → who you want to be.
- Current Me: "Edging all day"
- Ideal Me: "Business income"
- Bridges: "Business outreach 1hr/day"
- Duel the bridges to prioritize

### What is "Neural Forge"?
5-minute daily ritual to rewire your brain.
- Visualization (90s) = mental practice
- CBT challenge = test beliefs
- Micro-evidence = collect proof
- Streak = momentum

### What is "Phase"?
You transform in 3 phases:
- Phase 1 (0-30%): "Faking it" - feels unnatural
- Phase 2 (30-70%): "Believing it" - starting to stick
- Phase 3 (70-100%): "Being it" - automatic, natural

---

## 🎮 HOW DUELING WORKS

### Example Session

**Screen**: 
```
Left Card                Right Card
┌─────────────────────┬─────────────────────┐
│ Problem Solving     │ Technical Skills    │
│  ⚔️ vs ⚔️           │                     │
│  1200 Elo           │  1100 Elo           │
└─────────────────────┴─────────────────────┘
```

**You click**: Right (Technical Skills)
- Elo updates
- Win logged
- Next pair appears

**After 10 comparisons**:
```
🏆 Results:
1. Problem Solving (1250 Elo) ⭐⭐⭐
2. Technical Skills (1150 Elo) ⭐⭐
3. Leadership (980 Elo) ⭐
```

**Interpretation**: You care most about problem-solving.

---

## 📊 ANALYTICS EXPLAINED

### Stats on Dashboard

**Total Duels**: 187
- How many comparisons you've made
- More = better data clarity

**Phase %**: 34%
- Progress through transformation phases
- Each 10 micro-evidence = +1%
- Goal: Reach 100%

**Ritual Streak**: 7 🔥
- Days in a row completing Neural Forge
- Goal: 90+ day streak

**Peak Elo**: 1247
- Highest ranking across all items
- Shows strongest preference

---

## 🛠️ CHANGE YOUR PASSWORD

**IMPORTANT**: Default password is shown in code. Change it!

1. Tap "⚙️ Settings"
2. Scroll to bottom
3. See "Task Duel v8.0"
4. Look up above (top of page)
5. Right-click file → Edit
6. Find this line:
   ```
   const TASK_DUEL_PASSWORD = 'ChangeMeToYourPassword2025';
   ```
7. Change to your password:
   ```
   const TASK_DUEL_PASSWORD = 'MySecurePass123!';
   ```
8. Save → Re-upload to GitHub
9. Reload iPhone app
10. New password works!

---

## 💾 BACKUP YOUR DATA

### Daily Backup (Recommended)
```
1. "📈 Analytics" tab
2. "Backup" button
3. Sends .json file to Downloads
4. Move to Google Drive or iCloud
```

### What Gets Backed Up
- All duel history
- Forge quizzes completed
- Current/Ideal self items
- Neural stats (streak, evidence)
- All settings

### Restore from Backup
- Download .json file
- Open in text editor
- Copy content
- Settings → "Restore" button (future version)

---

## ❓ COMMON QUESTIONS

**Q: Is my data private?**
A: Yes. 100% stored on your iPhone in localStorage. Zero uploaded anywhere.

**Q: What if I delete the app?**
A: Data stays (iOS keeps localStorage). Reinstall and login.

**Q: Can I use on iPad/Mac?**
A: Yes! Same GitHub URL works. Data syncs if you use Netlify Identity (future).

**Q: How do I change password?**
A: Edit HTML file, find TASK_DUEL_PASSWORD line, change, re-upload.

**Q: Will updates delete my data?**
A: No. Update only changes code. localStorage data persists.

**Q: Can I export for Excel?**
A: Yes! "📈 Analytics" → "CSV" button downloads spreadsheet.

**Q: Is there a web version?**
A: Same link on desktop Safari = web version.

**Q: How many items can I compare?**
A: Unlimited. localStorage can hold ~5-10MB of data = 10,000+ duels.

---

## 🚨 TROUBLESHOOTING

### "Access Denied" after entering password
**Fix**: 
```
1. iPhone Settings → Safari → Advanced
2. "Clear History and Website Data"
3. Reopen app
4. Try password again
```

### Duel cards not clickable
**Fix**:
```
1. Refresh page (pull down in Safari)
2. Wait 2 seconds
3. Try again
```

### Forge quiz won't progress
**Fix**:
```
1. Make sure you clicked a suggestion OR typed in input
2. Click "Next" button
3. If stuck, refresh page
```

### Phone shows blank screen
**Fix**:
```
1. iPhone home screen
2. Settings → Safari
3. Disable "Block Pop-ups"
4. Reopen Task Duel
```

---

## 📈 SUCCESS METRICS

Track these to see transformation:

### Weekly
- [ ] 50+ duels completed
- [ ] 5+ Forge quizzes done
- [ ] 7 days Neural ritual streak

### Monthly
- [ ] 200+ total duels
- [ ] Phase % > 15%
- [ ] 3+ behavior changes initiated

### 3 Months
- [ ] 500+ duels
- [ ] Phase % > 50%
- [ ] Visible life changes
- [ ] New habits stuck

### 6 Months
- [ ] 1000+ duels
- [ ] Phase % > 80%
- [ ] Identity shift complete
- [ ] Goals achieved

---

## 🎓 UNDERSTANDING THE SCIENCE

Your app implements these proven brain-change mechanisms:

1. **Neuroplasticity**: Visualization rewires your brain
2. **Habit Stacking**: Daily Neural Forge builds automaticity
3. **Spaced Repetition**: Dueling over time = stronger learning
4. **Evidence Accumulation**: Small wins = big identity shift
5. **Identity-First**: You become what you duel for
6. **CBT**: Challenge limiting beliefs (Neural Forge)
7. **Embodied Cognition**: Your body learns what you prioritize

**The Loop**:
```
Duel (decide) → Evidence (collect) → Belief (form) → Action (do) → Result (achieve)
```

Repeat 100+ times = transformation.

---

## 🎯 EXAMPLE TRANSFORMATION PLAN

### Month 1: Brainstorm (Forge Phase)
```
Week 1: Do "Career" quiz → Get 10 job factors
Week 2: Do "Physical" quiz → Get 8 body goals
Week 3: Do "Dating" quiz → Get 12 sexual preferences
Week 4: Gap Bridge → Map current → ideal
```

### Month 2: Decision (Duel Phase)
```
Week 1: Duel 100 times (career items)
Week 2: Duel 100 times (physical items)
Week 3: Duel 50 times (dating items)
Week 4: Analytics → Review top 3 priorities
```

### Month 3: Execution (Neural Phase)
```
Week 1-4: Daily Neural Forge (5min ritual)
→ Every day: Visualization + CBT + Micro-evidence
→ Results: Phase % climbs from 0% → 35%
```

### Months 4-6: Integration
```
→ Continue Neural Forge daily
→ Add Gap Bridge actions (topping practice, business hours)
→ Phase % → 70-100%
→ Identity shift complete
```

---

## 🚀 NEXT STEPS

1. ✅ Download task-duel-v8.0.html
2. ✅ Deploy to GitHub Pages (2 min)
3. ✅ Add to iPhone home screen (1 min)
4. ✅ Change password (2 min)
5. ✅ Complete first Forge quiz (5 min)
6. ✅ Do 10 duels (10 min)
7. ✅ Start daily Neural Forge ritual (tomorrow morning)
8. ✅ Export your first backup (5 min)

**Total time to full setup: ~25 minutes**

---

## 💪 YOU'VE GOT THIS

You now have the most comprehensive personal transformation system available. 

**Remember**: 
- Small daily actions → Big transformation
- 100+ duels = clear pattern
- Neural Forge daily = brain rewiring
- Gap Bridge weekly = progress tracking
- Phase % climbing = real change

Your job: Keep playing. The app does the thinking.

**Deploy today. Transform by end of year. 🎉**

---

**Questions?** Everything's documented in CHANGELOG-v8.md

**Build Date**: December 5, 2025  
**Version**: 8.0  
**Status**: LIVE
