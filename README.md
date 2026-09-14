USJ Express Pass Finder & Day Itinerary Planner
An interactive, single-file web application built with Tailwind CSS, Lucide Icons, and Vanilla JavaScript to help Universal Studios Japan (USJ) visitors navigate complex ticketing rules, plan their daily itinerary, and match their desired rides to the exact official Express Pass packages.
---
💡 Motivation & Problem Solved
Booking tickets for Universal Studios Japan is notoriously difficult due to:
Area Timed Entry Tickets: Areas like Super Nintendo World frequently require timed digital entry passes that run out minutes after park gates open.
Express Pass Confusion: USJ sells multiple tiers and variants (Express 4, Express 5, Express 7, Express 8, and Premium) with rotating ride combinations, optional choice slots (`either one`), and seasonal lineups.
Overpaying vs. Long Queues: Guests often do not know which pass covers all the specific rides they care about without buying more expensive packages unnecessarily.
This project parses official USJ ticketing data, allows visitors to build a chronological daily schedule, and dynamically scores which Express Pass covers 100% of their selected attractions.
---
✨ Features
Live Express Pass Matching Engine:
Select your must-do rides and check ⚡ Request Express.
The engine cross-references the official catalog and sorts passes by match accuracy and lowest starting price.
Accurately resolves complex ticket mechanics such as optional ride slots (`MarioKart + Flying Dinosaur / Minion Mayhem (either one)`).
Explicitly highlights whether a pass guarantees Super Nintendo World Area Timed Entry.
Interactive Day Planner:
Add rides, shows, dining, or interactive merchandise experiences to a drag-free timeline.
Re-order items up/down to optimize physical movement across the park.
Set specific target times (e.g., `09:30`, `14:00`).
One-Click Markdown/Text Export:
Copy your planned schedule directly to your clipboard formatted as cleanly indented markdown bullets:
    ```text
    - 09:30 | Mario Kart: Koopa's Challenge (⚡ Express)
    - 11:00 | Mine Cart Madness (Donkey Kong) (⚡ Express)
    - 12:30 | Kinopio's Cafe (Toad Cafe)
    - 15:00 | Harry Potter and the Forbidden Journey (⚡ Express)
    ```
Comprehensive Park Directory:
Includes headliner attractions (Mario Kart, Mine-Cart Madness, Flying Dinosaur, Forbidden Journey).
Features live entertainment, seasonal Halloween events, and classic water shows (WaterWorld, NO LIMIT! Street Parade, Sing on Tour).
Filter by park zone (Super Nintendo World, Harry Potter, Minion Park, Jurassic Park, etc.).
Zero Dependencies & Zero Setup:
Runs completely in the browser via CDN assets. No `npm install`, Node.js, or backend servers required.
---
📦 Parsed Ticket Catalog
The internal dataset reflects official USJ ticketing products:
Pass Tier	Featured Inclusions	SNW Timed Entry?
Express ~Premium Unlimited~	All attractions, unlimited skip-the-line	Yes
Express Pass 8	Mine Cart, Mario Kart, Yoshi, Forbidden Journey, Hippogriff, Minion Blast, choice coasters	Yes
Express Pass 7	Mine Cart, Mario Kart, Yoshi, Forbidden Journey, Hippogriff, Flying Dino / Minion choice	Yes
Express Pass 5	Race & Minecart / Race & Minion / Adventure Special variants	Yes
Express Pass 4+1	Mario Kart (x2 rides), Forbidden Journey, Flying Dinosaur, Hollywood Dream	Yes
Express Pass 4 (Standard & Themed)	Race & JAWS, Theater & Flying Dino, Classic & Show (WaterWorld), Minions, etc.	Varies by package
Express Pass 4 (Halloween Specials)	Resident Evil Requiem, Chainsaw Man 4-D, Sadako's Curse, Factory of Fear	No (Event focused)
---
🚀 Quick Start
Clone the repository:
```bash
   git clone https://github.com/your-username/usj-pass-planner.git
   cd usj-pass-planner
   ```
Run the app:
Simply open `index.html` (or `usj_express_finder.html`) in any modern web browser:
```bash
   # On macOS
   open index.html

   # On Windows
   start index.html

   # On Linux
   xdg-open index.html
   ```
Alternatively, you can host it for free on GitHub Pages, Vercel, or Netlify with zero configuration.
---
🛠️ Tech Stack
HTML5 & Vanilla JavaScript (ES6+): Custom reactive state management for the timeline and matching engine.
Tailwind CSS (via CDN): Responsive utility-first interface styled for mobile and desktop screens.
Lucide Icons (via CDN): Lightweight SVG iconography.
---
⚠️ Disclaimer
This tool is an independent open-source project created for trip-planning purposes. It is not affiliated with, endorsed by, or associated with Universal Studios Japan, NBCUniversal, or JTRWeb LTD. Attraction lineups, heights, and ticket prices fluctuate by date and season; always verify real-time availability on the official USJ ticket portal prior to purchase.
