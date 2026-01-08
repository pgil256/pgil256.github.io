# Portfolio Marketability Redesign

**Date:** 2026-01-07
**Goal:** Make portfolio as marketable as possible for Software Engineer roles (primary), with Full-Stack and DevOps/SysAdmin as secondary positioning.

## Target

- **Primary role:** Software Engineer / Developer
- **Secondary:** Full-Stack, then DevOps/Infrastructure
- **Level:** Mid-level preferred, open to junior
- **Impression:** Professional, technical, and personable (balanced)

## Design Decisions

### 1. Hero Section

**Current:**
```
Patrick Gilhooley
System Administrator & Software Engineer
```

**New:**
```
Patrick Gilhooley
Software Engineer | Full-Stack & Systems
```

**Meta description:**
> Software Engineer with experience in full-stack development, embedded systems, and infrastructure automation.

**Rationale:** Lead with target role. SysAdmin experience shows in timeline but shouldn't be the headline.

---

### 2. About Section (New)

**Placement:** Between hero and experience sections.

**Content:**
> Former math teacher who discovered a passion for building software while automating classroom tasks. Now I build full-stack applications, embedded control systems, and infrastructure automation. I bring the same focus on clear communication and problem-solving to every engineering challenge.

**Rationale:** Frames career transition as intentional. Connects teaching skills (communication, problem-solving) to engineering value. Short enough to not be skipped.

---

### 3. Structure: Separate Experience & Projects

**Current:** Single "Experience & Projects" timeline mixing jobs and personal projects.

**New:** Two distinct sections.

#### Experience Section (Timeline)
- System Administrator @ Academie Da Vinci (May 2024 - Present)
- Software Engineer @ Ortho Integrative Medicine (Apr 2024 - Present)
- QA Engineer @ Coast Autonomous (Oct 2023 - Apr 2024)
- Secondary Math Instructor @ Pinellas County Schools (Sep 2019 - Sep 2023) — condensed

#### Projects Section (Card Grid)
- 2-column grid on desktop, 1-column on mobile
- Expandable to 3 columns with 6+ projects

**Rationale:** Recruiters scan differently for work history vs portfolio. Projects section can grow independently.

---

### 4. Project Card Format

Each card contains:
- **Title** — project name
- **One-liner** — what it does (not implementation details)
- **Tech badges** — 3-4 key technologies as pills/tags
- **Links** — GitHub, live demo if available

#### Current Projects

| Project | One-liner | Tech Stack |
|---------|-----------|------------|
| Juntas Seguras | Rotating savings pool platform | Next.js, TypeScript, MongoDB |
| Map My Seat | Classroom seating chart generator | React, Express, PostgreSQL |

#### Planned Additions

| Project | One-liner | Tech Stack |
|---------|-----------|------------|
| Home Finder | Pinellas County real estate aggregator | Django, Celery, PostgreSQL |
| TabVision | Guitar tab transcription from video | Electron, React, Flask, ML |
| DesktopPetPy | Windows desktop pet with AI behavior | Python, Pygame, Win32 |
| Weasel Entertainment System | Retro arcade game launcher | Python, Pygame, Raspberry Pi |

---

### 5. Skills Reorganization

**Current categories:** Languages & Backend, Databases & DevOps, Tools & Methods

**New categories:**

#### Languages
Python, TypeScript, JavaScript, C++, SQL, Bash

#### Frameworks & Libraries
React, Next.js, Django, Flask, Express, Node.js

#### Databases & Infrastructure
PostgreSQL, MongoDB, Docker, Git, Azure, CI/CD

**Removed:** Google Workspace, SQLite, JIRA, PyQt5 (less relevant for SWE roles)
**Added:** Next.js, Express, CI/CD (reflects actual project stack)

---

## Implementation Checklist

- [ ] Update hero title and tagline
- [ ] Update meta description
- [ ] Add About section after hero
- [ ] Split Experience & Projects into separate sections
- [ ] Convert Experience to timeline (4 roles)
- [ ] Convert Projects to card grid
- [ ] Style project cards with tech badges
- [ ] Reorganize skills into 3 new categories
- [ ] Test responsive layout
- [ ] Update footer year to 2025

---

## Files to Modify

- `index.html` — structure and content changes
- `css/style.css` — new styles for about section, project cards, tech badges
