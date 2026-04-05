# JHB City SDA Church — Bulletin App

Live PWA powered by Google Sheets. No redeployment needed for updates.

## 🔧 One-time setup

1. **Deploy to GitHub Pages** (do this once):
   - Create a new GitHub repo (e.g. `jhb-city-church`)
   - Upload `index.html`, `manifest.json`, `README.md`
   - Go to repo **Settings → Pages → Source: main branch → Save**
   - Your app is live at `https://YOUR-USERNAME.github.io/jhb-city-church`

2. **Set up Google Sheets** (do this once):
   - Create a new Google Sheet
   - Add 3 tabs named exactly: `config`, `announcements`, `contacts`
   - See column format below
   - Go to **File → Share → Publish to web → Entire Document → CSV → Publish**
   - Copy the URL and paste it into `index.html` where it says `YOUR_GOOGLE_SHEETS_CSV_URL_HERE`
   - Push the updated `index.html` to GitHub (last time you touch it!)

## 📊 Google Sheet format

### Tab: `config`
| key | value |
|-----|-------|
| banner | 📅 Sabbath, 4th April 2026 — Baptism Day |
| hero_title | Baptism & Holy Communion Day |
| hero_desc | Combined service with Betrams, Townsview & West Central |
| hero_badge | 📍 177 Commissioner St · 09:00–17:00 |
| verse_text | "Take, eat; this is My body…" |
| verse_ref | Matthew 26:26–29 |
| fundraiser_raised | R370.00 |
| fundraiser_goal | R6,000.00 |
| fundraiser_pct | 6.2 |

### Tab: `announcements`
| date | title | desc | type |
|------|-------|------|------|
| Apr 5, 2026 | Church Board Meeting | Sunday 5th April @ 14:00 | normal |
| Apr 11, 2026 | Guest & Music Day | Invite NON-SDA friends! | highlight |
| May 2, 2026 | Building Day | Sabbath Building Day | urgent |

> **type** = `normal`, `highlight` (gold), or `urgent` (red)

### Tab: `contacts`
| initials | role | name | phone |
|----------|------|------|-------|
| AM | Pastor | Alfred Mncube | +27 63 000 0206 |
| TN | Head Elder | Trey P. Ncube | +27 82 546 2906 |

## ✏️ Weekly workflow (admin)
1. Open your Google Sheet
2. Edit the `announcements` tab — add/remove rows
3. Update `config` tab for banner, hero, verse etc.
4. **Done.** The app refreshes automatically every 5 minutes for all users.

## 📱 Installing the app
Members open the link in Chrome/Safari → "Add to Home Screen" → installs as an app icon.
