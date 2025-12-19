# ��� Birthday Countdown Website

Beautiful birthday website with countdown, photo gallery, and celebration effects!

---

## ��� Quick Start

```bash
npm install
npm run dev
```
Open `http://localhost:5173`

---

## ✏️ Customize

### 1. Birthday Date ⏰

**File:** `src/components/Countdown.jsx` (Line 21)

```javascript
const targetDate = new Date("2026-07-21T00:00:00");
```

**Format Explanation:**
```
"YYYY-MM-DDTHH:MM:SS"
 ↓    ↓  ↓  ↓  ↓  ↓
 Year Mo Day Hr Min Sec
```

- **YYYY** = 4-digit year (2025, 2026, etc.)
- **MM** = 2-digit month (01=Jan, 02=Feb, ... 12=Dec)
- **DD** = 2-digit day (01 to 31)
- **T** = Separator (keep this!)
- **HH:MM:SS** = Time in 24-hour format

**Time Examples:**
| What you want | Use this |
|---------------|----------|
| Midnight (12:00 AM) | `00:00:00` |
| 9:00 AM | `09:00:00` |
| Noon (12:00 PM) | `12:00:00` |
| 3:30 PM | `15:30:00` |
| 11:59 PM | `23:59:00` |

**Real Examples:**
```javascript
// January 15, 2026 at midnight
const targetDate = new Date("2026-01-15T00:00:00");

// June 10, 2025 at 3:30 PM
const targetDate = new Date("2025-06-10T15:30:00");

// December 25, 2025 at noon
const targetDate = new Date("2025-12-25T12:00:00");
```
