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

## Multi-user

Stablix uses Supabase for authentication and cloud storage:

- Each user logs in with email and password
- Each user has their own separate horses and data
- An admin approves who gets access (hamburger menu → Users)
- All changes save automatically to the cloud

## Tech

- Pure HTML / CSS / JavaScript — one self-contained file
- Supabase — authentication and per-user cloud data storage
- CSS custom properties for the full colour theme
- Inline SVG icons, Google Fonts (DM Serif Display + DM Sans)
- `100dvh` layout, `safe-area-inset` padding — works correctly on iOS notch devices
- PWA-ready — add to home screen on iOS or Android for a full-screen native feel

## Navigation

- **Bottom bar** — Home, Calendar, Horses, Feeding plan
- **Hamburger menu** — full section list, export/import, users (admin), sign out
- **+ button** — context-sensitive add action from any screen
