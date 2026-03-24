# MakanPlan

A food-first trip planner built for real travel usage. Plan your meals, share your itinerary to WhatsApp in seconds.

**🔗 Live Demo → [lucysee.github.io/makanplan](https://lucysee.github.io/makanplan/)**

---
---

## App Flow

### 1. Create Trip Screen (First Page)
Always opens here on launch.

**Saved Trip card** (shown if a previous trip exists)
- Shows trip name, date range, stop count
- Status pill: 🗓 Upcoming / 🔥 Ongoing / ✓ Past
- Tap **Open Trip →** to continue planning
- Tap **🗑 Delete** to remove the trip (with confirmation)

**New Trip section**
- Enter a trip name (optional — auto-names from date if blank)
- Pick dates on the calendar — tap start date, then end date
- Single-day trip: tap the same date twice
- Button updates to show number of days selected
- Tap **Create X-Day Trip →** to begin

---

### 2. Planner Screen

**Day tabs** — one tab per day, auto-named with weekday and date (e.g. `Day 1 · Fri 17 Apr`)

**Adding food stops**

| Method | How |
|---|---|
| Quick Add | Tap ☕🍜🧋🍽🍡 — instant item, no typing |
| Paste Link | Tap 🔗 Paste Link → paste a Google Maps URL |

**Smart time defaults**
- First item uses meal-type defaults (Breakfast 08:30, Lunch 12:30, Cafe 15:30, Snack 17:00, Dinner 19:00)
- Subsequent items default to previous item time + 3 hours

**Item card shows**
- Time · Meal type emoji · Place name
- 📍 Maps button (if link added)
- 🍽 Dine-in or 🛵 GrabFood badge
- ✕ Delete button (always visible)

**Editing an item** — tap any card to open edit sheet
- Change time, place name, meal type, mode
- Paste or update Google Maps link (live preview opens link to verify)
- Add notes
- 🗑 Delete button inside sheet

---

### 3. WhatsApp Share

Tap the green **Share** button → opens WhatsApp with a formatted itinerary:

```
🍜 KUANTAN
━━━━━━━━━━━━━━━━━━━━

📅 DAY 1 · FRI 17 APR
─────────────────────

12:30  🍜 Lunch
📍 Loteng Cafe Telok Cempedak
🗺 maps.google.com/...
🍽 Dine-in

18:00  🍽 Dinner
📍 Chicken rice
🛵 GrabFood delivery

━━━━━━━━━━━━━━━━━━━━
Planned with MakanPlan 🍜
```

---

## Data

- Saved to browser `localStorage` — persists between sessions on the same device
- One active trip at a time
- Deleting a trip is permanent (confirmation required)

---

## Meal Types & Defaults

| Type | Emoji | Default Time |
|---|---|---|
| Breakfast | ☕ | 08:30 |
| Lunch | 🍜 | 12:30 |
| Cafe | 🧋 | 15:30 |
| Snack | 🍡 | 17:00 |
| Dinner | 🍽 | 19:00 |

---

## File

`index.html` — the entire app in one file.

---

*Built with plain HTML, CSS, and JavaScript. No frameworks. No dependencies. No internet required.*
