# ⚔️ Task-Duel Masterblock - Quick Reference Guide

## 🎮 Controls & Shortcuts

| Key(s) | Action |
|--------|--------|
| `←` or `A` | Select left card |
| `→` or `D` | Select right card |
| `U` | Undo last comparison |
| `Space` or `Enter` | Confirm (future) |
| `🌙` button | Toggle dark mode |

## 🎯 Core Workflow

### 1. **Create a Duel Session**
   - Go to **📊 Dashboard** tab
   - Select a preset OR click **➕ Create Custom Session**
   - Choose items to duel
   - Session starts automatically

### 2. **Make Comparisons**
   - See two cards side-by-side
   - Click a card OR use keyboard shortcuts (`A`/`D` or `←`/`→`)
   - Watch:
     - ✨ **Elo delta badge** shows Elo gain/loss
     - 📊 **Progress ring** (top-right) animates forward
     - 🔄 **Mini previous card** appears between cards

### 3. **Edit Previous Comparisons**
   - Hover over the mini card in the middle
   - See "Click to rewind" tooltip
   - Click to undo and reselect that comparison
   - OR press `U` to undo last comparison

### 4. **Complete Session**
   - Answer all comparisons
   - 🎊 **Confetti celebration** + modal with:
     - 🥇 Top 3 winners with Elo ratings
     - 📊 Total comparisons made
     - ⏱️ Average decision time
   - View full results in **🏆 Results** tab

---

## 🌙 Dark Mode

**Toggle:** Click the sun/moon icon (☀️ / 🌙) in the header top-right

**Auto-saves:** Your preference persists across page reloads

**Covers:** All UI elements, cards, modals, and backgrounds

---

## 📊 Progress Ring

**Location:** Fixed in top-right corner (always visible)

**Shows:** 
- Percentage complete
- "Complete" label
- Animated circle fill

**Updates:** Every time you select an option

---

## ✨ Elo Delta Badge

**When:** Appears after you click a card

**Shows:** `+X Elo` (green) or `-X Elo` (red)

**Duration:** Animates upward and fades over 1.2 seconds

**Purpose:** Visualize ranking impact of your choice

---

## 🎯 Mini Previous Card

**Location:** Between the two main comparison cards (middle column)

**Shows:** Last comparison result with winner highlighted

**Interact:** 
- Hover to see "Click to rewind" tooltip
- Click to undo and re-select that comparison
- OR press `U` key to undo

**Visual:** Includes left accent bar (colored by winner)

---

## 🎊 Completion Celebration

**Triggers:** When all comparisons in a session complete

**Shows:**
1. 🎉 **Confetti animation** (colored particles falling)
2. 📋 **Modal with stats:**
   - Total comparisons made
   - Average decision time
   - Items ranked
   - Top 3 winners (🥇 🥈 🥉) with Elo scores

**Then:** View full rankings in **🏆 Results** tab

---

## 💾 Data Persistence

**Auto-save:** Enabled by default (see ⚙️ Settings)

**Stores:**
- All comparisons and results
- Item Elo ratings
- Session history
- Dark mode preference
- Keyboard shortcut preference

**Backup:** Download data in **💾 Memory** tab

---

## ⚙️ Settings (Optional)

**Access:** ⚙️ **Settings** tab

**Configurable:**
- Elo K-Factor (default: 32)
- Keyboard shortcuts (enabled/disabled)
- Auto-save (enabled/disabled)

---

## 🏆 Results & History

**Results Tab:**
- See current rankings by Elo
- Filter by category
- Export data

**History Tab:**
- View all past sessions
- See comparison details
- Replay sessions

---

## 🔗 Integrations (Demo)

**Notion:** 
- Connect your Notion database
- Import tasks for dueling
- Sync results back

*(Note: Demo version. Production requires API setup)*

---

## ⌨️ Pro Tips

1. **Speed Run:** Use keyboard shortcuts (`A`/`D`) instead of clicking—5x faster!
2. **Edit Mistakes:** Pressed wrong key? Press `U` to undo instantly
3. **Night Mode:** Dark mode is easy on eyes—toggle with 🌙 button
4. **Track Progress:** Watch the circular progress ring—satisfying feedback!
5. **Review Winners:** Check the 🏆 Results tab after each session
6. **Rewind:** Click mini cards to edit/rewind and re-select comparisons

---

## 🐛 Troubleshooting

**Q: Progress ring not updating?**  
A: Refresh page. Ensure auto-save is enabled in ⚙️ Settings.

**Q: Dark mode not saving?**  
A: Check browser localStorage is enabled.

**Q: Keyboard shortcuts not working?**  
A: Enable in ⚙️ Settings → Keyboard Shortcuts checkbox.

**Q: Confetti not showing?**  
A: If completion modal appears, confetti canvas should animate. Check browser console for errors.

---

## 📝 Notes

- All data saves to `localStorage` (browser storage)
- Clear browser storage to reset app
- Data persists across sessions by default
- Sessions can be exported/imported via Memory tab

---

**Version:** 2.0 with 6 UX Improvements  
**Last Updated:** December 4, 2025  
**Features:** 🎊 Confetti • 📊 Progress Ring • ✨ Elo Badges • 🎯 Mini Hover • 🌙 Dark Mode • ⌨️ Shortcuts
