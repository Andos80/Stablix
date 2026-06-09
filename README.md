# Stablix

A mobile-first stable management app built as a single HTML file — no frameworks, no build step.

**Live:** https://andos80.github.io/Stablix

## What it does

Stablix helps you track everything that matters for a small stable:

- **Horses** — profile cards with breed, lineage, coat colour, and photo; per-horse health, activities, files, and feeding plan
- **Activities** — log training sessions, vet checks, and treatments (flatwork, jumping, hacking, shows, massage, and more)
- **Health** — vaccination, farrier, and dentist records with status indicators and next-appointment dates
- **Calendar** — monthly grid with per-horse colour bars; add and manage events
- **Feeding plan** — per-horse meal plans for breakfast, lunch, and dinner with hay, compound feeds, and supplements
- **Costs** — expense tracking per horse with category breakdown
- **Notes** — journal per horse
- **Files** — photos, videos, and documents per horse

## Language

Stablix supports Norwegian and English. Switch between them with the flag button in the top bar — all UI text, labels, and activity types update instantly. The preference is saved per device.

## Multi-user

Stablix uses Supabase for authentication and cloud storage:

- Each user logs in with email and password
- Forgot your password? Use the "Forgot password?" link on the sign-in screen — a reset link is sent to your email
- Each user has their own separate horses and data
- An admin approves who gets access (hamburger menu → Users)
- All changes save automatically to the cloud
- Data syncs across devices — log in from any browser or phone

## Privacy

Stablix stores your email address to provide access to the service. Data is processed in accordance with GDPR. To request deletion of your account and data, contact the stable owner.

## Tech

- Pure HTML / CSS / JavaScript — one self-contained file
- Supabase — authentication and per-stable cloud data storage (raw fetch against REST API for reliability)
- CSS custom properties for the full colour theme
- Inline SVG icons, Google Fonts (DM Serif Display + DM Sans)
- `100dvh` layout, `safe-area-inset` padding — works correctly on iOS notch devices
- PWA-ready — add to home screen on iOS or Android for a full-screen native feel

## Navigation

- **Bottom bar** — Home, Calendar, Horses, Feeding plan
- **Hamburger menu** — full section list, export/import, users (admin), sign out
- **+ button** — context-sensitive add action from any screen
- **Flag button** — toggle between Norwegian and English
- **Sun/moon button** — toggle between light and dark mode
