# Portfolio Projects

## Juntas Seguras

### Summary
A platform for managing community savings pools, also known as ROSCAs (Rotating Savings and Credit Associations) or "tandas." Groups of trusted members contribute a fixed amount on a regular schedule (weekly, bi-weekly, or monthly), and each round one member receives the full pool as a payout. The cycle continues until everyone has received their turn. The app handles pool creation, member management, contribution tracking, payout scheduling, and communication between members through discussion threads with @mentions.

### Tech Stack
- **Frontend:** Next.js 14, React 18, TypeScript, Tailwind CSS, shadcn/ui
- **Backend:** Next.js API Routes, NextAuth.js (JWT authentication)
- **Database:** MongoDB with Mongoose ODM
- **Security:** Mandatory MFA (email-based or TOTP authenticator), Stripe Identity for KYC verification
- **Features:** Zelle QR code generation, payment deep links (Venmo, PayPal, Zelle, Cash App), audit logging, email notifications

### Links
- **Live:** [https://juntas-seguras.vercel.app](https://juntas-seguras.vercel.app)
- **GitHub:** [https://github.com/pgil256/juntas-seguras](https://github.com/pgil256/juntas-seguras)

---

## Map My Seat

### Summary
A seating chart generator built for K-12 teachers. Educators input their class rosters, define their classroom's physical layout (rows, columns, table arrangements), and specify seating preferences or constraints. The app then generates an optimized seating arrangement that can be saved, modified, and exported as PDF. Designed to save teachers the time typically spent manually arranging students.

### Tech Stack
- **Frontend:** React 18, Vite, Chakra UI, React Router v6
- **Backend:** Node.js, Express.js
- **Database:** PostgreSQL with Knex.js query builder and Objection.js ORM
- **Authentication:** JWT with bcrypt password hashing
- **Features:** PDF export (jsPDF, html2canvas), CSV import for student rosters

### Links
- **Live:** [https://map-my-seat.vercel.app](https://map-my-seat.vercel.app)
- **GitHub:** [https://github.com/pgil256/map-my-seat-flyio](https://github.com/pgil256/map-my-seat-flyio)

---

## Home Finder

### Summary
A property search tool that aggregates real estate data for Pinellas County, Florida. The app scrapes and consolidates information from two official government sources: the Pinellas County Property Appraiser (property details, valuations, square footage, year built) and the Tax Collector (tax amounts, payment status, delinquencies). Users can search by city, ZIP code, property type, and price range, then export results as Excel, PDF, or CSV reports.

### Tech Stack
- **Backend:** Django 5.0, Python 3.12, Django REST Framework, Celery with Redis
- **Data Collection:** Selenium WebDriver (headless Chrome) for web scraping
- **Data Processing:** Pandas, OpenPyXL (Excel), ReportLab (PDF), Matplotlib (charts)
- **Frontend:** Tailwind CSS, Webpack
- **Features:** Async task processing for large datasets (400k+ parcels), real-time progress tracking, email notifications

### Links
- **Live:** [https://web-production-0e103.up.railway.app](https://web-production-0e103.up.railway.app)
- **GitHub:** [https://github.com/pgil256/home_finder](https://github.com/pgil256/home_finder)
