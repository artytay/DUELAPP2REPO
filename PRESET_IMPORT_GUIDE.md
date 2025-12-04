# 📥 Preset Import Guide

## Overview

The Task-Duel app now supports **importing custom presets** that you can generate externally with AI or create manually. This allows you to:

- 🤖 Generate preset configurations using AI tools (ChatGPT, Claude, etc.)
- 📋 Import presets from external sources
- 💾 Export your custom presets for sharing or backup
- 🔄 Reuse presets across different devices

---

## Quick Start

### Importing a Preset

1. **Navigate to Dashboard** → Click the **📥 Import Preset** button
2. **Select a JSON file** containing your preset configuration
3. **Review the preview** to ensure everything looks correct
4. **Click Import Preset** to add it to your app
5. **Use your preset** by clicking "⚔️ Start Duel" in the Quick Start Presets section

### Exporting Presets

1. **Go to Dashboard** → Click the **📤 Export Presets** button
2. **Choose an option:**
   - **Export ALL presets**: Downloads all your presets in one file
   - **Export template**: Downloads a format guide for creating new presets with AI
3. **Use the exported file** to back up, share, or import into another instance

---

## Preset File Format

Presets must be valid JSON files with the following structure:

```json
{
  "title": "My Preset Name",
  "description": "A brief description of what this preset is for",
  "items": [
    {
      "name": "First Item",
      "description": "Optional description for item 1"
    },
    {
      "name": "Second Item",
      "description": "Optional description for item 2"
    },
    {
      "name": "Third Item",
      "description": "Optional description for item 3"
    }
  ]
}
```

### Requirements:

- ✅ Must have a `title` field (string)
- ✅ Must have an `items` array with **at least 2 items**
- ✅ Each item must have a `name` field (string)
- ✅ Optional: `description` for both preset and items
- ✅ Valid JSON format

### Example - Job Search Preferences:

```json
{
  "title": "💼 Ideal Job Criteria",
  "description": "Rank the most important factors in your job search",
  "items": [
    {
      "name": "Salary & Compensation",
      "description": "Total comp including benefits"
    },
    {
      "name": "Remote Work Options",
      "description": "Flexibility to work from home"
    },
    {
      "name": "Growth Opportunities",
      "description": "Career advancement potential"
    },
    {
      "name": "Work-Life Balance",
      "description": "Reasonable hours and flexibility"
    },
    {
      "name": "Team Culture",
      "description": "Collaborative and supportive environment"
    },
    {
      "name": "Meaningful Work",
      "description": "Projects that feel impactful"
    }
  ]
}
```

---

## Using AI to Generate Presets

You can use AI tools like ChatGPT, Claude, or Copilot to generate presets. Here's a sample prompt:

### Prompt Template:

```
Generate a Task-Duel preset in JSON format for [your topic].

Requirements:
- Topic: [describe what you want to rank]
- Number of items: [e.g., 8-10]
- Include descriptive text for each item

Format:
{
  "title": "...",
  "description": "...",
  "items": [
    {"name": "...", "description": "..."},
    ...
  ]
}

Only output the JSON, no other text.
```

### Example Prompts:

**1. Learning Goals**
```
Generate a Task-Duel preset in JSON format for ranking programming languages to learn.
Include 8 popular languages with brief descriptions.
Format as shown above. Only output JSON.
```

**2. Vacation Planning**
```
Generate a Task-Duel preset to help someone choose their next vacation destination.
Include 10 different destinations with descriptions of their highlights.
Format as shown above. Only output JSON.
```

**3. Project Priorities**
```
Generate a Task-Duel preset for a product manager to rank feature requests.
Include 12 potential features with brief descriptions of value/effort.
Format as shown above. Only output JSON.
```

---

## Step-by-Step: Creating a Preset with AI

### Step 1: Write Your Prompt

```
Generate a Task-Duel preset in JSON format for comparing coffee brewing methods.
Include at least 6 different brewing methods (pour over, espresso, French press, etc.).
Each should have a name and a description explaining the method.

Output only valid JSON in this exact format:
{
  "title": "Coffee Brewing Methods",
  "description": "Compare and rank different ways to make coffee",
  "items": [
    {"name": "Method Name", "description": "Brief description"}
  ]
}
```

### Step 2: Copy AI Response

Copy the JSON output from the AI.

### Step 3: Save to File

Save the JSON in a `.json` file (e.g., `coffee-preset.json`)

### Step 4: Import into Task-Duel

1. Go to Dashboard
2. Click "📥 Import Preset"
3. Select your file
4. Review preview
5. Click "Import Preset"
6. Start dueling!

---

## Preset Structure Explained

### Required Fields

| Field | Type | Example |
|-------|------|---------|
| `title` | String | "🎓 Skills to Learn" |
| `items` | Array | [ { "name": "...", "description": "..." } ] |

### Item Fields

| Field | Type | Required | Example |
|-------|------|----------|---------|
| `name` | String | ✅ Yes | "Public Speaking" |
| `description` | String | ❌ Optional | "Present to audiences" |

### Optional Preset Fields

| Field | Type | Default | Example |
|-------|------|---------|---------|
| `description` | String | "" | "Rank skills to prioritize learning" |

---

## Common Use Cases

### 1. **Decision Making**
- Compare job offers
- Choose a vacation destination
- Select a programming language to learn

### 2. **Priority Ranking**
- Product feature requests
- Bug fix priorities
- Task prioritization

### 3. **Personal Development**
- Skills to develop
- Personal values ranking
- Habits to build

### 4. **Team Exercises**
- Feature prioritization meetings
- Team values alignment
- Project planning

### 5. **Comparative Analysis**
- Software tools comparison
- Business models
- Investment options

---

## Troubleshooting

### "Invalid file format" Error

**Solution:** Ensure your JSON is valid:
- Use a JSON validator: https://jsonlint.com/
- Check for missing commas or quotes
- Verify all brackets are matched

### "Preset must contain at least 2 items" Error

**Solution:** Add more items to your preset's `items` array.

### "Missing title or items array" Error

**Solution:** Ensure your JSON has:
- A `title` field (string)
- An `items` field (array)

### File Won't Upload

**Solution:**
- Make sure file has `.json` extension
- Check file size (should be small)
- Try a different browser if issue persists

---

## Tips & Tricks

### 💡 Tip 1: Use Emojis in Titles

Emojis make presets more visually appealing:
```json
"title": "🎬 Movie Night Choices"
```

### 💡 Tip 2: Detailed Descriptions

Better descriptions help during dueling:
```json
{
  "name": "Work-Life Balance",
  "description": "Reasonable hours, vacation time, and flexibility"
}
```

### 💡 Tip 3: Even Number of Items

Use an even number of items (6, 8, 10, 12) for more balanced comparisons.

### 💡 Tip 4: Export Templates

Export the template option to share with team members as an example format.

### 💡 Tip 5: Batch Import

You can import multiple presets one at a time. Each import adds to your preset library.

---

## Exporting Your Presets

### Why Export?

- **Backup:** Save your custom presets
- **Share:** Send presets to teammates
- **Reuse:** Import same presets on different devices
- **Archive:** Keep a record of preset variations

### How to Export

1. Go to Dashboard
2. Click "📤 Export Presets"
3. Choose:
   - **All Presets:** Downloads everything
   - **Template:** Downloads format guide
4. File saves to your Downloads folder
5. Share or backup as needed

---

## Advanced: Creating Complex Presets

### Using AI for Complex Analysis

**Prompt Example:**
```
Generate a Task-Duel preset to help someone decide between 8 different cities 
to live in. For each city, provide:
- A compelling name/title
- 2-3 key factors that make it unique (cost, culture, weather, job market, etc.)

Format as JSON with name and description fields.
```

### Preset for Group Decisions

```json
{
  "title": "🤝 Team Meeting Agenda Items",
  "description": "Help the team prioritize what to discuss",
  "items": [
    {"name": "Q1 Planning", "description": "Quarterly goals and roadmap"},
    {"name": "Budget Review", "description": "Department budget discussion"},
    {"name": "Team Building", "description": "Organize team outing"},
    {"name": "Process Improvements", "description": "Ways to improve workflows"}
  ]
}
```

---

## FAQ

**Q: Can I edit a preset after importing?**
A: Yes! Click "✏️ Edit Items" on any preset to modify items.

**Q: Can I delete an imported preset?**
A: Currently, you can remove items from a preset. To completely remove a preset, you would need to export data, edit the JSON, and re-import.

**Q: How many presets can I import?**
A: Unlimited! All presets are stored locally in your browser.

**Q: Will my presets sync across devices?**
A: Currently, presets are stored locally per device. Export and import to transfer between devices.

**Q: Can I share my preset file?**
A: Yes! Export your presets and share the `.json` file with others to use.

**Q: What if the AI generates invalid JSON?**
A: Ask the AI to validate the JSON or paste it into https://jsonlint.com/ to find errors.

---

## Example Presets to Try

### Fitness Routine Priority
```json
{
  "title": "🏋️ Fitness Goals",
  "description": "Rank what's most important in your routine",
  "items": [
    {"name": "Build Muscle", "description": "Strength training focus"},
    {"name": "Cardio Endurance", "description": "Running and stamina"},
    {"name": "Flexibility", "description": "Yoga and stretching"}
  ]
}
```

### Content Topics
```json
{
  "title": "📝 Blog Post Ideas",
  "description": "Decide what to write about next",
  "items": [
    {"name": "Tutorial: React Hooks"},
    {"name": "Guide: Time Management"},
    {"name": "Review: New Framework"}
  ]
}
```

---

## Need More Help?

- Check the in-app Settings tab for general help
- Review the imported preset preview before confirming import
- Make sure your JSON is valid using an online JSON validator

Enjoy creating and importing presets! 🚀
