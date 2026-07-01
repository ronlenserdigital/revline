# REVLINE — live car meet map (MVP)

A single-page web app for car communities: everyone opens it at a meet or cruise, picks
their car, and sees the crew on a live map with real-time speed, plus group chat.

- **Stack:** Leaflet + OpenStreetMap (free maps), Supabase Realtime (free presence + broadcast). No build step, no server.
- **Deploy:** static host over HTTPS (Vercel recommended). GPS requires HTTPS.

## Setup
1. Create a free project at supabase.com.
2. Project Settings → API → copy the **Project URL** and **anon public** key.
3. In `index.html`, replace `YOUR_SUPABASE_URL` and `YOUR_SUPABASE_ANON_KEY` in the config block.
4. Optionally change `ROOM` to run separate rooms per meet/city.
5. Deploy to Vercel and share the HTTPS link.

## Status
Validation MVP. Foreground-only tracking, no accounts, chat/presence are not persisted.
Native (Expo) build with background tracking + accounts comes only after demand is proven.
