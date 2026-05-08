# Portfolio Projects

## KneeSpa Control System

### Summary
Embedded control system for a medical knee decompression device. Raspberry Pi operator software coordinates a PyQt5 GUI, Arduino serial control, GPIO e-stop handling, and three motion axes with real-time pressure feedback. The companion DRX simulator mirrors the device firmware protocol in a browser-based 3D demo for protocol testing and product demonstrations.

### Tech Stack
- **Device control:** Python, PyQt5, C++, Arduino serial protocol
- **Hardware:** Raspberry Pi, Arduino, GPIO e-stop, pressure sensors, three-axis actuator control
- **Simulator:** Vite, React, TypeScript, Three.js, React Three Fiber, Zustand, Tailwind CSS

### Links
- **Website:** [https://kneespa.com/providers/](https://kneespa.com/providers/)
- **Demo:** [https://drx-simulator.patbuilds.dev](https://drx-simulator.patbuilds.dev)
- **Simulator GitHub:** [https://github.com/pgil256/drx-simulator](https://github.com/pgil256/drx-simulator)

---

## Juntas Seguras

### Summary
Secure platform for managing community savings pools, also known as ROSCAs or tandas. Groups create pools, invite members, track contributions, schedule payouts, and communicate through discussion threads with @mentions. Security features include mandatory MFA, Stripe Identity verification, audit logging, payment reminders, and support workflows.

### Tech Stack
- **Frontend:** Next.js 14.2, React 18, TypeScript, Tailwind CSS, shadcn/ui
- **Backend:** Next.js App Router API routes, NextAuth.js JWT authentication
- **Database:** MongoDB with Mongoose ODM
- **Security and payments:** MFA, Stripe Identity, payment method tracking, audit logging

### Links
- **Live:** [https://juntasseguras.patbuilds.dev](https://juntasseguras.patbuilds.dev)
- **GitHub:** [https://github.com/pgil256/juntas-seguras](https://github.com/pgil256/juntas-seguras)

---

## Map My Seat

### Summary
Automated seating chart generator for K-12 teachers. Teachers import rosters, design classroom layouts, set keep-apart and seat-together rules, mark accommodations, and run a simulated-annealing solver that generates scored seating charts. The app supports drag-to-swap edits, per-desk rationale tooltips, CSV import, PDF export, and a no-signup demo mode.

### Tech Stack
- **Frontend:** React 18, Vite, Chakra UI, React Router v6
- **Backend:** Node.js, Express.js, JSON Schema validation
- **Database:** PostgreSQL with Knex.js migrations
- **Authentication:** JWT with bcrypt password hashing
- **Testing:** Jest, Vitest, React Testing Library

### Links
- **Live:** [https://mapmyseat.patbuilds.dev](https://mapmyseat.patbuilds.dev)
- **GitHub:** [https://github.com/pgil256/map-my-seat-flyio](https://github.com/pgil256/map-my-seat-flyio)

---

## Home Finder

### Summary
Searchable index of 437,000+ Pinellas County, Florida property records from the official County Property Appraiser dataset. A monthly GitHub Actions import loads bulk county data into Neon Postgres, and the Django app serves fast indexed search, detail pages, market statistics, Google Street View cards, and Excel/PDF exports from Vercel serverless functions.

### Tech Stack
- **Web:** Django 5.0, Python 3.12, Vercel serverless
- **Database:** Neon Postgres with indexed city, type, and market value queries
- **Frontend:** Tailwind CSS, Webpack, Django templates
- **Data refresh:** GitHub Actions scheduled import
- **Testing:** Playwright, pytest, httpx, GitHub Actions CI

### Links
- **Live:** [https://homefinder.patbuilds.dev](https://homefinder.patbuilds.dev)
- **GitHub:** [https://github.com/pgil256/home_finder](https://github.com/pgil256/home_finder)

---

## TabVision

### Summary
Automatic guitar tab transcription from video. TabVision fuses Basic Pitch audio detection with MediaPipe hand tracking so the app can infer not only what pitch was played, but where it was played on the fretboard. The output is a synced tab editor with confidence scoring, inline correction, plain-text export, and PDF export.

### Tech Stack
- **Desktop client:** Electron 28, React 18, Zustand, Tailwind CSS
- **Backend:** Python 3.11, Flask, async job queue
- **Audio:** Basic Pitch, ffmpeg
- **Video:** MediaPipe Hands, OpenCV
- **Fusion:** Custom pitch and hand-position scoring

### Links
- **Live:** [https://tabvision.patbuilds.dev](https://tabvision.patbuilds.dev)
- **GitHub:** [https://github.com/pgil256/tab_vision](https://github.com/pgil256/tab_vision)
