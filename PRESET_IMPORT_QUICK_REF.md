# 📥 Quick Reference: Importing Presets

## One-Minute Overview

**What:** Import pre-built comparison lists into Task-Duel  
**Why:** Use AI to generate presets or import from other sources  
**How:** Dashboard → 📥 Import Preset → Select JSON file → Done!

---

## Minimal JSON Format

The absolute simplest preset:

```json
{
  "title": "My Preset",
  "items": [
    {"name": "Option A"},
    {"name": "Option B"},
    {"name": "Option C"}
  ]
}
```

**That's it!** Descriptions are optional.

---

## Complete JSON Format

With all optional fields:

```json
{
  "title": "My Preset Title",
  "description": "What this preset is for",
  "items": [
    {"name": "Item 1", "description": "Details about item 1"},
    {"name": "Item 2", "description": "Details about item 2"},
    {"name": "Item 3", "description": "Details about item 3"}
  ]
}
```

---

## Validation Checklist

Before importing, verify:

- [ ] File is `.json` format
- [ ] Has `"title"` field
- [ ] Has `"items"` array
- [ ] At least 2 items in array
- [ ] Each item has `"name"` field
- [ ] Valid JSON (use https://jsonlint.com/)

---

## AI Prompts - Copy & Paste Ready

### Generic Template
```
Generate a Task-Duel preset in JSON format for [TOPIC].
Include [NUMBER] items with descriptions.
Output ONLY valid JSON in this format:
{
  "title": "...",
  "description": "...",
  "items": [{"name": "...", "description": "..."}]
}
```

### Example: Learning Goals
```
Generate a Task-Duel preset for choosing Python data science libraries to learn.
Include 8 libraries. Output only JSON.
```

### Example: Career Decisions
```
Generate a Task-Duel preset to compare job offers.
Include salary, benefits, growth, work-life balance, culture, location, and remote work options.
Output only JSON.
```

---

## How to Import (3 Steps)

1. **Click** "📥 Import Preset" in Dashboard
2. **Select** your `.json` file
3. **Confirm** when preview looks good

File appears in Quick Start Presets instantly!

---

## How to Export

1. **Click** "📤 Export Presets" in Dashboard
2. **Choose:**
   - **All Presets** = Everything you created/imported
   - **Template** = Format guide for creating new ones
3. **File downloads** to your computer

---

## Common Formats

### Decision Making (6-8 items)
```
[Option A, Option B, Option C, ...]
```

### Rankings (8-12 items)
```
[Item 1, Item 2, Item 3, ...]
```

### Prioritization (5-10 items)
```
[Priority A, Priority B, Priority C, ...]
```

---

## Troubleshooting

| Problem | Solution |
|---------|----------|
| "Invalid JSON" | Use https://jsonlint.com/ to validate |
| "Need 2+ items" | Add more items to the array |
| "Missing title" | Ensure `"title": "..."` exists |
| "File won't upload" | Use `.json` extension |

---

## Real Examples You Can Copy

### Fitness Goals
```json
{
  "title": "🏋️ Fitness Goals",
  "items": [
    {"name": "Build Muscle"},
    {"name": "Increase Cardio"},
    {"name": "Improve Flexibility"}
  ]
}
```

### Coffee Methods
```json
{
  "title": "☕ Brewing Methods",
  "items": [
    {"name": "Pour Over"},
    {"name": "French Press"},
    {"name": "Espresso"},
    {"name": "AeroPress"}
  ]
}
```

### Tech Stack
```json
{
  "title": "💻 Web Frameworks",
  "items": [
    {"name": "React"},
    {"name": "Vue.js"},
    {"name": "Svelte"},
    {"name": "Angular"}
  ]
}
```

---

## Pro Tips

✨ **Tip 1:** Use emojis in titles  
`"title": "🎬 Movie Night"`

✨ **Tip 2:** Add detailed descriptions  
`"description": "What should we watch?" `

✨ **Tip 3:** Even numbers of items (6, 8, 10)

✨ **Tip 4:** Export your presets for backup

✨ **Tip 5:** Share preset files with teammates

---

## File Management

**Save as:** `my-preset.json`

**Location:** Downloads folder (or anywhere)

**Share:** Email the `.json` file to others

**Keep:** Export regularly for backup

---

## Getting Started with AI

### ChatGPT Prompt:
```
Create a Task-Duel preset in JSON format to help me 
choose between [topic]. Include 8 options.
Output ONLY valid JSON.
```

### Claude Prompt:
```
Generate JSON for a Task-Duel preset comparing 
[topic]. 8-10 items with descriptions please.
```

### Copilot Prompt:
```
Make a JSON preset file for Task-Duel that ranks
[topic]. Include at least 6 options.
```

---

## Limits & Support

- **Storage:** Unlimited (local browser storage)
- **Devices:** Export/import to use across devices
- **Sharing:** Share `.json` files via email
- **Backup:** Regularly export your presets

---

**Start importing presets today! 🚀**

Need help? Check `PRESET_IMPORT_GUIDE.md` for detailed instructions.
