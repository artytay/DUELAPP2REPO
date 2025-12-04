# 📋 Preset JSON Schema & Validation Rules

## Official Schema

```json
{
  "$schema": "http://json-schema.org/draft-07/schema#",
  "title": "Task-Duel Preset Format",
  "type": "object",
  "required": ["title", "items"],
  "properties": {
    "title": {
      "type": "string",
      "description": "Name of the preset",
      "minLength": 1,
      "maxLength": 200,
      "examples": ["My Preset", "🎯 Career Choices"]
    },
    "description": {
      "type": "string",
      "description": "Optional description of what this preset is for",
      "minLength": 0,
      "maxLength": 500,
      "default": "",
      "examples": ["Help me decide on career paths", ""]
    },
    "items": {
      "type": "array",
      "description": "Array of items to compare",
      "minItems": 2,
      "maxItems": 100,
      "items": {
        "type": "object",
        "required": ["name"],
        "properties": {
          "name": {
            "type": "string",
            "description": "Item name",
            "minLength": 1,
            "maxLength": 200,
            "examples": ["Option A", "Decision B"]
          },
          "description": {
            "type": "string",
            "description": "Optional item description",
            "minLength": 0,
            "maxLength": 500,
            "default": "",
            "examples": ["Details about this item", ""]
          }
        }
      }
    }
  },
  "additionalProperties": false
}
```

---

## Validation Rules

### Required Fields

| Field | Type | Min Length | Max Length | Example |
|-------|------|-----------|-----------|---------|
| `title` | string | 1 char | 200 chars | "My Preset" |
| `items` | array | 2 items | 100 items | [...] |
| item `name` | string | 1 char | 200 chars | "Option A" |

### Optional Fields

| Field | Type | Default | Max Length | Example |
|-------|------|---------|-----------|---------|
| `description` | string | "" | 500 chars | "Description" |
| item `description` | string | "" | 500 chars | "Details" |

### Constraints

✅ **Must have:**
- `title` (non-empty string)
- `items` array (2 or more items)
- Each item must have `name`

❌ **Cannot have:**
- Empty title
- Less than 2 items
- Items without names
- Invalid JSON syntax

---

## Complete Valid Examples

### Minimal (Simplest)
```json
{
  "title": "My Choices",
  "items": [
    {"name": "A"},
    {"name": "B"}
  ]
}
```

**Valid?** ✅ YES (all required fields)

---

### Complete (All Fields)
```json
{
  "title": "Career Decision",
  "description": "Help me choose between job offers",
  "items": [
    {
      "name": "Startup Position",
      "description": "High growth, equity, uncertain hours"
    },
    {
      "name": "Corporate Job",
      "description": "Stable, good benefits, bureaucratic"
    },
    {
      "name": "Freelance",
      "description": "Freedom, variable income, solo work"
    }
  ]
}
```

**Valid?** ✅ YES (has all optional fields too)

---

### With Emojis (Great for UX)
```json
{
  "title": "🎯 Skills to Learn",
  "description": "Which programming skill should I prioritize?",
  "items": [
    {"name": "🐍 Python", "description": "AI, data science, automation"},
    {"name": "🦀 Rust", "description": "Systems, performance, safety"},
    {"name": "💛 Go", "description": "Cloud, microservices, concurrency"},
    {"name": "🎯 Zig", "description": "Low-level control, bare metal"}
  ]
}
```

**Valid?** ✅ YES (emojis are fine!)

---

## Invalid Examples (Don't Do This!)

### ❌ Missing Title
```json
{
  "items": [
    {"name": "A"},
    {"name": "B"}
  ]
}
```
**Error:** ❌ Missing required field `title`

---

### ❌ Empty Items Array
```json
{
  "title": "My Preset",
  "items": []
}
```
**Error:** ❌ Items array must have at least 2 items

---

### ❌ Only One Item
```json
{
  "title": "My Preset",
  "items": [
    {"name": "Only Option"}
  ]
}
```
**Error:** ❌ Need minimum 2 items to compare

---

### ❌ Item Without Name
```json
{
  "title": "My Preset",
  "items": [
    {"description": "This item has no name"},
    {"name": "Item B"}
  ]
}
```
**Error:** ❌ Each item must have a `name` field

---

### ❌ Invalid JSON Syntax
```json
{
  "title": "My Preset",
  "items": [
    {"name": "A"},
    {"name": "B"},  // <- trailing comma
  ]
}
```
**Error:** ❌ Invalid JSON (trailing comma not allowed)

---

### ❌ Wrong Data Types
```json
{
  "title": 123,
  "items": "not an array"
}
```
**Error:** ❌ Title must be string, items must be array

---

## Validation Checklist

Use this to verify your preset before importing:

```
☐ File has .json extension
☐ Valid JSON (no syntax errors)
☐ Has "title" field (non-empty string)
☐ Has "items" field (array)
☐ Items array has 2 or more items
☐ Each item has "name" field
☐ No trailing commas
☐ All quotes are double quotes (not single)
☐ All braces { } and brackets [ ] match
☐ No extra fields not in schema
```

---

## Auto-Validation When Importing

The app will check:

1. **JSON Syntax** → Valid JSON format?
2. **Required Fields** → Has title + items?
3. **Array Length** → At least 2 items?
4. **Item Structure** → Each item has name?
5. **String Fields** → All strings are valid?

Errors shown immediately in the modal.

---

## Validation Error Messages

| Error | Cause | Fix |
|-------|-------|-----|
| "Invalid preset format: missing title or items array" | No title or items field | Add both fields |
| "Preset must contain at least 2 items" | Less than 2 items | Add more items |
| "Item 0 missing or invalid 'name' field" | Item has no name | Add name to each item |
| "Invalid JSON" | Syntax error | Use JSON validator |
| "Cannot read property 'items'" | JSON parsing failed | Check JSON syntax |

---

## Testing Your JSON

### Method 1: Use Online Validator
https://jsonlint.com/
1. Paste your JSON
2. Click "Validate JSON"
3. Shows errors clearly

### Method 2: Use Browser Console
```javascript
try {
  JSON.parse(yourJsonString);
  console.log("✅ Valid JSON");
} catch (e) {
  console.log("❌ Invalid JSON:", e.message);
}
```

### Method 3: Use Text Editor
Many editors highlight JSON errors:
- VS Code
- Sublime Text
- Atom
- NotePad++

---

## Best Practices

### ✅ DO:
- Use descriptive titles
- Include meaningful descriptions
- Use 6-12 items for best results
- Use consistent formatting
- Test with validator before importing
- Keep names concise
- Use emojis for visual appeal
- Export regularly for backup

### ❌ DON'T:
- Leave descriptions empty if possible
- Use single quotes instead of double quotes
- Add extra fields not in schema
- Use trailing commas
- Mix data types
- Create presets with only 1 item
- Use special characters improperly
- Forget to validate before importing

---

## Common Formatting Mistakes

### ❌ Single Quotes (Wrong)
```json
{
  'title': 'My Preset',  // ← Wrong! Use double quotes
  'items': [
    {'name': 'A'}
  ]
}
```

### ✅ Double Quotes (Right)
```json
{
  "title": "My Preset",  // ✅ Correct
  "items": [
    {"name": "A"}
  ]
}
```

---

### ❌ Trailing Commas (Wrong)
```json
{
  "title": "My Preset",
  "items": [
    {"name": "A"},
    {"name": "B"},  // ← Trailing comma not allowed
  ]  // ← Extra comma here too
}
```

### ✅ No Trailing Commas (Right)
```json
{
  "title": "My Preset",
  "items": [
    {"name": "A"},
    {"name": "B"}  // ✅ No comma after last item
  ]
}
```

---

## Size Limits

| Constraint | Limit | Reason |
|-----------|-------|--------|
| Title length | 200 chars | Display purposes |
| Description length | 500 chars | Modal display |
| Item name length | 200 chars | UI constraints |
| Item description | 500 chars | Card display |
| Number of items | 100 max | Performance |
| Total file size | No limit* | Browser storage |

*Limited by browser localStorage (typically 5-10MB)

---

## Format Variations

### Variation 1: Minimal Format
```json
{"title":"X","items":[{"name":"A"},{"name":"B"}]}
```
**Size:** ~40 bytes | **Valid?** ✅ YES

### Variation 2: Standard Format
```json
{
  "title": "X",
  "items": [
    {"name": "A"},
    {"name": "B"}
  ]
}
```
**Size:** ~60 bytes | **Valid?** ✅ YES

### Variation 3: Full Format
```json
{
  "title": "X",
  "description": "Desc",
  "items": [
    {"name": "A", "description": "Desc A"},
    {"name": "B", "description": "Desc B"}
  ]
}
```
**Size:** ~120 bytes | **Valid?** ✅ YES

All are valid! Use whatever is most readable for you.

---

## Schema Compliance

This schema complies with:
- ✅ JSON Schema Draft 7
- ✅ UTF-8 encoding
- ✅ Standard JSON format
- ✅ No custom extensions

---

## Extending the Schema (Future)

Possible future fields (not yet supported):
- `category` - Preset category
- `tags` - Search tags  
- `difficulty` - Easy/Medium/Hard
- `author` - Who created it
- `version` - Schema version
- `createdAt` - Timestamp
- `updatedAt` - Timestamp

For now, stick to: `title`, `description`, `items`

---

## Quick Validation Template

Copy and modify:

```json
{
  "title": "YOUR_TITLE_HERE",
  "description": "YOUR_DESCRIPTION_HERE",
  "items": [
    {"name": "Item 1", "description": "Description 1"},
    {"name": "Item 2", "description": "Description 2"},
    {"name": "Item 3", "description": "Description 3"}
  ]
}
```

1. Replace `YOUR_TITLE_HERE`
2. Fill in items
3. Test with validator
4. Import!

---

**Your preset is valid when it matches this schema!** ✅
