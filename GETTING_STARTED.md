# 🚀 Getting Started: Import Your First Preset

## You're All Set! Here's What's New

Your Task-Duel app now has **preset import functionality**. This means you can:

- ✨ Use AI to generate comparison lists
- 📥 Import them directly into the app
- 🎯 Start dueling immediately
- 📤 Export for backup or sharing

---

## Try It Right Now (30 seconds)

### Option 1: Use the Example Presets

1. **Look for** `example-presets.json` in your app folder
2. **Go to Dashboard tab** in your app
3. **Click "📥 Import Preset"** button (new!)
4. **Choose** `example-presets.json`
5. **See the preview** of the startup ideas preset
6. **Click "Import Preset"**
7. **Done!** It now appears in your presets

### Option 2: Create Your Own with AI

**Copy this prompt** and paste into ChatGPT/Claude:

```
Generate a Task-Duel preset in JSON format for choosing a new hobby.
Include 8 different hobbies with brief descriptions.
Output ONLY valid JSON in this exact format:
{
  "title": "My Hobby",
  "description": "Choose a new hobby",
  "items": [
    {"name": "Hobby Name", "description": "Why this hobby"}
  ]
}
```

**Steps:**
1. Copy the response (the JSON part only)
2. Save it as `my-hobbies.json`
3. Open your app → Dashboard
4. Click "📥 Import Preset"
5. Choose your file
6. Confirm and you're done!

---

## What Files You Have

### 📚 Documentation Files (Read These!)

| File | Purpose | Read Time |
|------|---------|-----------|
| `PRESET_IMPORT_GUIDE.md` | **Complete guide** with everything | 15 min |
| `PRESET_IMPORT_QUICK_REF.md` | **Quick reference** - most useful | 5 min |
| `example-presets.json` | **7 ready-to-use presets** | 0 min |

### 💡 Start Here

👉 **Read:** `PRESET_IMPORT_QUICK_REF.md` (takes 5 minutes)

Then:
- Try the example presets
- Generate one with AI
- Import and start dueling!

---

## Common Scenarios

### Scenario 1: "I want AI to help me decide"

```
1. Think of a decision you need to make
2. Ask AI to generate a Task-Duel preset about it
3. Copy the JSON response
4. Save as .json file
5. Import into app
6. Let the app help you decide!
```

**Example AI Prompt:**
```
Create a JSON preset to help me choose between these job offers:
- Job A: High salary, commute
- Job B: Remote, less pay  
- Job C: Startup equity, growth
- Job D: Stable, benefits

Include these factors for each: salary, flexibility, growth, culture, security.

Output as Task-Duel JSON format only.
```

### Scenario 2: "I want to share presets with my team"

```
1. Build your custom presets in the app
2. Click "📤 Export Presets"
3. Choose "All Presets"
4. Share the JSON file via email/Slack
5. Team members import it
6. Everyone gets the same presets!
```

### Scenario 3: "I want to back up my presets"

```
1. Go to Dashboard
2. Click "📤 Export Presets"
3. Download your file
4. Store it safely
5. Can import anytime!
```

---

## The Format (Super Simple)

### Minimum Required:
```json
{
  "title": "My Preset",
  "items": [
    {"name": "Option 1"},
    {"name": "Option 2"},
    {"name": "Option 3"}
  ]
}
```

### With Descriptions (Better):
```json
{
  "title": "My Preset",
  "description": "What this is for",
  "items": [
    {"name": "Option 1", "description": "Why option 1"},
    {"name": "Option 2", "description": "Why option 2"}
  ]
}
```

That's all! Just valid JSON.

---

## Pro Tips

💡 **Tip 1: Use Emojis**
```json
"title": "🎯 My Preset"
```

💡 **Tip 2: Detailed Descriptions**
```json
"items": [
  {
    "name": "Full Name Here",
    "description": "Be specific about why this matters"
  }
]
```

💡 **Tip 3: Even Numbers**
Use 6, 8, 10, or 12 items for best results

💡 **Tip 4: Back It Up**
Export your presets monthly

💡 **Tip 5: Share with Team**
Export and email to colleagues

---

## Quick Links to Resources

### 📖 Full Documentation
- `PRESET_IMPORT_GUIDE.md` - Complete guide with everything

### 📋 Quick Reference  
- `PRESET_IMPORT_QUICK_REF.md` - One-page cheat sheet

### 📁 Example Files
- `example-presets.json` - 7 ready presets (import immediately!)

### 📝 This File
- You're reading the "Getting Started" guide

---

## Next Steps

### Right Now (5 minutes)
- [ ] Import `example-presets.json`
- [ ] Try one of the example presets
- [ ] Complete a practice duel

### Today (30 minutes)
- [ ] Read `PRESET_IMPORT_QUICK_REF.md`
- [ ] Generate a preset with AI
- [ ] Import your custom preset
- [ ] Start a real duel session

### This Week
- [ ] Try 3-4 different presets
- [ ] Share with a friend or colleague
- [ ] Export your presets as backup

---

## Troubleshooting

**Q: File won't upload?**
A: Make sure it ends with `.json` and is valid JSON

**Q: "Invalid format" error?**
A: Check that it has `title` and `items` fields

**Q: Want to validate JSON?**
A: Use https://jsonlint.com/

**Q: How do I know if my preset is good?**
A: Preview shows before import - make sure it looks right!

---

## Need Help?

1. **Check:** `PRESET_IMPORT_QUICK_REF.md` (copy-paste ready)
2. **Read:** `PRESET_IMPORT_GUIDE.md` (complete guide)
3. **Try:** `example-presets.json` (working examples)

---

## Success Checklist

- ✅ Found the "📥 Import Preset" button
- ✅ Read one of the documentation files
- ✅ Imported a preset (example or your own)
- ✅ Saw it appear in Quick Start Presets
- ✅ Started a duel with imported preset
- ✅ Now you're ready to rank anything!

---

## What You Can Do Now

🎯 **Rank Decisions**
- Job offers
- Vacation destinations  
- Career paths
- Product features

📊 **Prioritize**
- Project tasks
- Feature requests
- Learning goals
- Habits to develop

🤝 **Team Exercises**
- Feature prioritization
- Value alignment
- Planning sessions
- Decision making

💡 **Generate Ideas**
- Ask AI for preset ideas
- Get structured comparisons
- Make better decisions
- Discover hidden preferences

---

## Ready to Start?

### Option A: Quick Start (2 min)
```
1. Import example-presets.json
2. Try a preset
3. Complete a duel
```

### Option B: Custom (10 min)
```
1. Generate preset with AI
2. Save as .json
3. Import
4. Duel
```

### Option C: Learn First (15 min)
```
1. Read PRESET_IMPORT_QUICK_REF.md
2. Review examples
3. Try a preset
4. Generate your own
```

---

**You're all set! Enjoy your enhanced Task-Duel app! 🚀**

Questions? Check the documentation files provided.

Happy dueling! ⚔️
