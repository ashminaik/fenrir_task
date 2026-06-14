# uhzmi_games: Locally Hosted Browser Game Portal with Admin Panel

**Category:** Web Development

---

## Context

Uhzmi Games needs a locally runnable, single page game portal where a visitor can browse, search, and play free HTML5 games instantly with no login. All game data lives in local JSON files and the site runs fully offline on localhost. A minimal admin panel lets the owner add, edit, or delete games through a simple form. This milestone covers the full portal: a dark themed React and Vite front end plus a tiny Node.js Express backend used only by the admin panel.

The freelancer also sources and integrates 12 free license itch.io games so the portal is populated from day one. The site has no user accounts, no database, and no internet dependency once the initial npm install is done. The entire portal runs through a single npm run dev command, and every game file, cover, JSON file, and the admin panel is self contained inside the project folder.

---

## Project Information

| Field | Details |
|---|---|
| Project ID | uhzmi_games |
| Category | Web Development |
| Project Type | Locally Hosted Single Page Browser Game Portal with Admin Panel |
| Client / Brand | Uhzmi Games |
| Industry | Gaming, Independent Game Studio |
| Location | Bangalore, India |
| Contact | hello@uhzmigames.com |
| Platform / Medium | React 18 with Vite single page application, runs on localhost, desktop browser plus mobile browser |
| Deliverable Type | .zip archive of the full project folder |
| Primary Goal | Ship a dark themed React portal that browses, searches, and plays 12 self hosted HTML5 games, with a minimal Express admin panel to add, edit, and delete games. |

---

## Main Goal

Deliver a locally runnable, dark themed single page game portal built with React 18 and Vite that reads all game data from local JSON files served by a minimal Node.js Express backend. A visitor can browse game cards by category, view the Top 5 Most Played, search games by title, sort and filter a category, open a dedicated game page, and play the game inside an iframe. The site owner can add, edit, and delete games through a minimal admin panel at /admin with no login. The whole portal runs offline on localhost through a single npm run dev command after one npm install.

1. A homepage with a Top 5 Most Played carousel, one carousel row per category, and a Browse All Games grid of every game.
2. Category pages with five sort options and tag filtering.
3. A game play page that loads each game into an iframe, with related games and a breadcrumb.
4. A search experience with live autocomplete.
5. A minimal admin panel at /admin to add, edit, and delete games, backed by an Express server that writes to games.json.
6. Twelve real itch.io HTML5 games fully integrated, plus 12 covers and 2 sound files.

---

## About Uhzmi Games

Uhzmi Games is an independent game studio and digital entertainment publisher founded in 2024, based in Bangalore, India. The studio curates and publishes browser based casual games. This portal is a locally hosted product: it has no user accounts, no database, and no internet dependency once npm install is done.

**Brand identity:** dark navy interface, violet purple primary accent #7C3AED, an animated dot field background, and an animated ASCII style logo.

---

## Requirements

### Core Functionality

1. The portal is a single page application built with React 18 and Vite, runnable on localhost with npm run dev.
2. All game data is read from local JSON files in src/data/ (games.json, categories.json, sounds.json) through a single dataService.js abstraction.
3. A minimal Node.js Express server (server.js) reads and writes games.json for the admin panel only.
4. The site runs fully offline on localhost after the initial npm install. No database, no user accounts, no internet dependency at runtime.
5. The site has four persistent regions on every page: a sticky top header, a left sidebar, a main content area, and a footer.
6. Twelve free license HTML5 games sourced from itch.io are integrated and populated in games.json from day one.
7. Adding a game requires only dropping a game folder, a cover image, and one JSON entry, with no code changes.

### Stack

- Frontend framework: React 18 with Vite.
- Local backend: Node.js with Express, minimal, admin panel only.
- Data storage: local JSON files (games.json, categories.json, sounds.json).
- Styling: Tailwind CSS.
- Animated background: reactbits.dev DotField component.
- Animated logo: reactbits.dev AsciiText component.
- Game embedding: HTML iframe from the local /games/ folder.
- Package manager: npm.
- Font: Inter (Google Fonts, free and open source).
- Icons: Lucide React (free and open source).
- Sounds: free CC0 or CC-BY audio from Freesound.org or Mixkit.co.

### Overall Page Structure (four persistent regions)

1. Top Header: sticky, stays pinned while content scrolls underneath. Animated AsciiText "Uhzmi Games" logo on the left, primary navigation links (Games, Categories, New, Popular) in the center, a search bar on the right, and a background music toggle button on the far right.
2. Left Sidebar: a vertical list of all twelve categories with small icons. The active category is highlighted in the accent color. On mobile, the sidebar collapses into a hamburger menu that slides in from the left.
3. Main Content Area: a scrollable region with the DotField animated background and game content overlaid on top, organized into horizontal sections.
4. Footer: a multi column layout with links to About, FAQ, Terms of Use, Privacy Policy, Contact, and a copyright line.

### Header

- Sticky, stays pinned to the top of the viewport during scroll.
- Animated AsciiText logo rendering "UHZMI GAMES" on the left in white or the accent color.
- Primary navigation links in the center: Games, Categories, New, Popular.
- A search bar with a magnifying glass icon on the right.
- A background music toggle button (speaker icon) on the far right.

### Left Sidebar

- A vertical list of all twelve categories from categories.json, each with a small icon.
- The active category is highlighted in the accent color #7C3AED.
- On mobile, the sidebar collapses into a hamburger menu that slides in from the left.

### Main Content Area

- A scrollable region containing the DotField animated background.
- All game cards, the sidebar, and text content sit on top with appropriate backgrounds or semi transparent panels so content stays readable.
- Organized into horizontal sections.

### Footer

- A multi column layout, five columns on desktop, stacked on mobile.
- Five link sections, each opening its content as a static page or modal overlay: About, FAQ, Terms of Use, Privacy Policy, Contact.
- A copyright line below the columns.

### Footer Content (use exactly as written in the PRD, do not modify)

Copyright line (below the columns): (c) 2026 Uhzmi Games. All rights reserved.

About:
Uhzmi Games is an independent game studio founded in 2024, based in Bangalore, India. We curate and publish browser based casual games [...] (complete this paragraph from the PRD verbatim).

FAQ:
Q: Do I need to install anything to play?
A: No. All games run directly in your browser. Just click a game card and start playing.
Q: What browser works best?
A: Chrome, Firefox, Edge, and Safari all work fine. Keep your browser updated for the best experience.
Q: Can I play on mobile?
A: Yes. The site is fully responsive and works on phones and tablets. Some games may play better with a keyboard on desktop.
Q: Are these games safe?
A: Yes. All games are free of malware and run in a sandboxed browser environment. We source games from trusted platforms with verif [...] (complete from the PRD verbatim).
Q: Can I submit my own game?
A: This portal is locally hosted. If you have the project files, you can add your game by following the instructions in the project [...] (complete from the PRD verbatim).

Terms of Use:
By using the Uhzmi Games portal, you agree to the following terms:
1. All games are provided "as is" for entertainment purposes only. Uhzmi Games makes no guarantees about game availability, perform [...] (complete from the PRD verbatim).
2. Games hosted on this portal are sourced under open licenses (MIT, GPL, CC0, or free to use). If you are a game developer and bel [...] (complete from the PRD verbatim).
3. You may not attempt to modify, reverse engineer, or redistribute the games or the portal software without explicit permission.
4. Uhzmi Games is not responsible for any damages or losses resulting from the use of this portal.
5. These terms may be updated at any time. Continued use of the portal after changes means you accept the new terms.

Privacy Policy:
Last updated: June 2026
This portal runs entirely on your local machine. It does not collect, store, or transmit any personal data.
What we do NOT collect:
- No names, email addresses, or account information (there are no user accounts).
- No IP addresses or location data (the site runs offline on localhost).
- No browsing history or game play data (play counts are stored only in a local JSON file on your machine).
- No cookies (the site only uses localStorage for the background music toggle preference, which never leaves your browser).
Third party services:
- Google Fonts (Inter font) is loaded from Google's CDN when the site first loads. Google may log the font request as per their privacy policy.
- reactbits.dev components are installed locally via npm and do not make external requests at runtime.
If you have questions about privacy, contact hello@uhzmigames.com.

Contact:
Email: hello@uhzmigames.com
Location: Bangalore, India
Response time: We aim to reply within 2 business days.
For game submissions, licensing inquiries, or general questions, send us an email. Since this portal is locally hosted, please incl [...] (complete from the PRD verbatim).

### Homepage Sections (in order, top to bottom)

1. Top 5 Most Played Games: a horizontal featured row showing the five games with the highest playCount. Each card is slightly larger than standard cards. The row is a carousel with left and right arrow buttons that appear on hover.
2. Category Rows: one row per category from categories.json. Each row has a bold heading and a "See all" link that routes to the full category page. Each row is a horizontal carousel. Arrows appear on row hover and scroll the row, and hide at the start and end extents. Rows that have zero games are hidden.
3. All Games Section: a "Browse All Games" heading followed by a static wrapped grid showing every game on the site, sorted newest first by default.

### Game Card Design

- A rounded corner rectangle with a 16:9 cover image filling most of the card.
- Game title below the thumbnail in white Inter font, weight 600.
- Optional corner badge ribbon: New, HOT, or Top Rated in accent colors.
- A metadata row below the title showing star rating and play count.

### Game Card Hover States

On mouse hover, the card does all of the following at once with a 200ms ease in out transition:

1. Scales up to transform: scale(1.05) so the card pops above its neighbors.
2. Shows an elevated drop shadow through a growing box shadow.
3. Raises z-index so the zoomed card overlaps adjacent cards instead of being clipped.
4. Fades in a dark semi transparent gradient overlay over the thumbnail.
5. Shows a centered white play icon (triangle) on top of the overlay.
6. Brightens the title text or shifts it to the accent color.
7. On mouse leave, everything reverses smoothly over the same 200ms with no instant snap.

On mobile and touch devices, hover effects are disabled and tapping navigates directly to the game page.

### Category Pages

- Reached from the left sidebar or the "See all" link on each homepage row.
- A full width grid of game cards filtered to that category.
- Sort and filter controls at the top:
  - Most Popular: sorted by playCount descending.
  - Newest First: sorted by addedDate descending.
  - Oldest First: sorted by addedDate ascending.
  - A to Z: sorted alphabetically by title ascending.
  - Z to A: sorted alphabetically by title descending.
  - Tag filter: clicking a tag shows all games with that tag within the current category.
- Infinite scroll or a "Load More" button as the user scrolls down.

### Search

- A search bar in the header with a magnifying glass icon.
- A live autocomplete dropdown as the user types, debounced 250ms.
- Matching game titles appear with small thumbnail images.
- Enter or clicking a suggestion navigates to the game page or the search results page.
- Arrow keys move through suggestions, Esc closes the dropdown, and clicking outside closes it.

### Game Play Page

- Reached by clicking any game card. URL pattern: /games/[slug].
- A large central game viewport with a loading spinner while the game boots.
- A click to play splash overlay before the game loads.
- A player toolbar with a Fullscreen toggle (browser Fullscreen API) and a report button.
- Below the viewport: game title, developer or author name, a short description, and controls or instructions.
- A related games grid below with six to eight similar games from the same category and tags.
- A breadcrumb trail: Home > Category Name > Game Title.
- No rating widget, no comments, no favorites.

### Top 5 Most Played Logic

- The playCount field in games.json increments by 1 on the Node.js server every time a user clicks to start a game.
- On homepage load, the frontend reads the top five games sorted by playCount descending and shows them in the featured carousel.
- Counts persist as long as games.json is not reset.

### Sound and Audio

- Card Click Sound: a short click or pop, roughly 0.1 to 0.3 seconds, non intrusive, that plays when the user clicks any game card. Sourced from Freesound.org under CC0.
- Background Music: a looping ambient or light electronic track that plays softly while browsing. A header toggle (speaker icon) turns it on and off. The toggle state persists in localStorage. Default state is off. Sourced from Mixkit.co under free license.
- Both files live in public/sounds/ as click.mp3 and bgm.mp3. The sounds.json file maps these filenames.

### Admin Panel (Method A, the easy way)

A minimal admin panel at /admin, local only, with no login and no authentication. It has three functions.

Add a Game: a form with these fields. Submitting writes a new entry to games.json.
- Title (text, slug auto generates from the title as you type and shows below the field as a preview).
- Category (dropdown, pulls options from categories.json).
- Tags (text, comma separated, for example "shooting, 3d, fps").
- Description (textarea, one to two sentences shown on the game page).
- Controls (text, for example "WASD to move, mouse to aim").
- Author (text, developer or studio name).
- Source (text, for example "itch.io" or "self-made").
- License (text, for example "MIT" or "CC0").
- Badge (dropdown, options: None, New, HOT, Top Rated).
- Game folder path (text, the slug name of the folder already placed in /games/).
- Cover image path (text, the slug name of the cover already placed in /public/covers/).

Edit a Game: a table listing all current games with an Edit button. Editing opens the same form prefilled with that game data. Submitting updates that entry in games.json.

Delete a Game: a Delete button next to each game removes the entry from games.json. It does not delete the game folder or cover image from disk.

Technical requirements: runs at /admin on localhost only, the form submits via POST to the Express server in server.js, the server reads and writes games.json on the local file system, no authentication is required, and a functional UI is sufficient.

### Manual Game Addition (Method B, for advanced users)

The fallback if the admin panel is not working, or for batch adding multiple games.

1. Drop the game folder into /games/[slug]/ with index.html at the root.
2. Drop the cover image into /public/covers/[slug].jpg (640x360, 16:9, JPG).
3. Open src/data/games.json.
4. Add a new JSON object following the schema below.
5. Save the file and refresh the site.

The README must document both Method A and Method B in detail under a section called "Adding a New Game", including the exact JSON schema, field descriptions, folder naming rules, and common troubleshooting tips.

### JSON Data Files

The freelancer must create these files in src/data/. All content below is final and used as is.

categories.json:
```json
[
  { "id": "action",      "label": "Action",      "icon": "icon-action.svg" },
  { "id": "racing",      "label": "Racing",      "icon": "icon-racing.svg" },
  { "id": "adventure",   "label": "Adventure",   "icon": "icon-adventure.svg" },
  { "id": "puzzle",      "label": "Puzzle",      "icon": "icon-puzzle.svg" },
  { "id": "sports",      "label": "Sports",      "icon": "icon-sports.svg" },
  { "id": "arcade",      "label": "Arcade",      "icon": "icon-arcade.svg" },
  { "id": "shooting",    "label": "Shooting",    "icon": "icon-shooting.svg" },
  { "id": "strategy",    "label": "Strategy",    "icon": "icon-strategy.svg" },
  { "id": "simulation",  "label": "Simulation",  "icon": "icon-simulation.svg" },
  { "id": "board",       "label": "Board Games", "icon": "icon-board.svg" },
  { "id": "music",       "label": "Music",       "icon": "icon-music.svg" },
  { "id": "educational", "label": "Educational", "icon": "icon-educational.svg" }
]
```

games.json entry schema (template, replace values with the actual itch.io game details):
```json
{
  "id": 1,
  "title": "Shadow Strike 3D",
  "slug": "shadow-strike-3d",
  "cover": "covers/shadow-strike-3d.jpg",
  "category": "action",
  "tags": ["shooting", "3d", "fps"],
  "description": "Infiltrate enemy bases and take down targets with precision in this fast-paced 3D shooter.",
  "controls": "WASD to move, mouse to aim, left-click to shoot, R to reload.",
  "gameUrl": "games/shadow-strike-3d/index.html",
  "badge": "HOT",
  "author": "StrikeDev Studios",
  "source": "itch.io",
  "license": "MIT",
  "addedDate": "2026-06-13",
  "playCount": 0
}
```

sounds.json:
```json
{
  "cardClick": "sounds/click.mp3",
  "backgroundMusic": "sounds/bgm.mp3",
  "enabled": false
}
```

### Responsiveness

- The grid reflows to 2 columns on mobile viewport widths.
- The left sidebar collapses into a hamburger menu that slides in from the left on mobile.
- Hover effects are disabled on touch devices, and tapping a card navigates directly to the game page.
- The site is fully responsive and works on phones and tablets.

### Accessibility

- Buttons have a visible focus ring in the accent color with a 2px outline offset for keyboard accessibility.
- Every image element carries an alt attribute.
- Content stays readable over the animated background through solid or semi transparent panels.

> Rule for this section: the palette, the pixel sizes, the counts, the file names, and the JSON content are the source of truth for the rubric. Every fixed value above is testable.

---

## Game Catalogue (12 itch.io Games)

The freelancer populates games.json with twelve real HTML5 games sourced from itch.io. Each game must be free to download and carry a license that allows self hosting (MIT, GPL, CC0, or free to use), and must run fully in a browser from its own index.html with no external server.

Required games, one per category:

1. Action: an FPS or shooting game.
2. Racing: a drifting or kart racing game.
3. Adventure: a dungeon crawler or maze escape game.
4. Puzzle: a block, tile, or word puzzle game.
5. Sports: a football or soccer game with local multiplayer.
6. Arcade: a space shooter or brick breaker game.
7. Shooting: a sniper or target shooting game.
8. Strategy: a tower defense or turn based strategy game.
9. Simulation: a city builder or management simulation game.
10. Board Games: chess, checkers, or any board based game.
11. Music: a rhythm or music creation game.
12. Educational: a math, typing, or learning game.

For each game, the freelancer must:

- Download the game zip from itch.io.
- Rename the folder to the game slug (lowercase, hyphens only).
- Place it in /games/[slug]/ with index.html at the root.
- Source the cover image from the game itch.io page.
- Resize or crop the cover to 640x360 pixels (16:9) and save as JPG.
- Place the cover in /public/covers/[slug].jpg.
- Create the matching entry in games.json with all fields filled.
- Document the source URL and license in the README.

Substitution rule: if a game type is unavailable on itch.io, the freelancer may substitute a functionally equivalent game in the same category that meets all license requirements. Substitutions must be approved by the project owner before integration.

---

## Visual & Technical Specs

### Dimensions / Sizing

- **Game card cover thumbnail:** 16:9 aspect ratio.
- **Cover image files:** 640 by 360 pixels, JPG, named by slug.
- **Card click sound length:** 0.1 to 0.3 seconds.
- **Mobile grid:** 2 columns.
- **Card hover scale:** 1.05.
- **Card hover transition:** 200ms ease in out.
- **Button hover transition:** 150ms ease.
- **Button active state:** scale 0.97 to 0.98, opacity 0.9, 100ms.
- **Button focus ring:** 2px outline offset in the accent color.

### Typography

Inter from Google Fonts is used for all text on the site.

| Element | Weight | Size |
|---|---|---|
| Site logo (AsciiText) | n/a | Large display |
| Section headings | 700 Bold | 24px |
| Card titles | 600 SemiBold | 16px |
| Body text and descriptions | 400 Regular | 14px |
| Metadata (play count, rating) | 400 Regular | 12px |
| Nav links | 500 Medium | 14px |

### Colors

These exact hex values are used throughout the entire site.

| Usage | Hex | Description |
|---|---|---|
| Page Background | `#0A0E1A` | Dark navy, main background behind the DotField animation |
| Card Background | `#141829` | Slightly lighter, used for game cards, sidebar, and content panels |
| Primary Text | `#FFFFFF` | White, all headings and main text |
| Secondary Text | `#8892B0` | Muted grey blue, metadata, descriptions, footer text |
| Accent Color | `#7C3AED` | Violet purple, logo hover, active nav links, button backgrounds, card hover title color, play icon |
| Badge HOT | `#EF4444` | Red badge ribbon |
| Badge New | `#22C55E` | Green badge ribbon |
| Badge Top Rated | `#F59E0B` | Gold or amber badge ribbon |
| Overlay Gradient | `rgba(0, 0, 0, 0.55)` | Dark overlay that fades in on card hover |
| Sidebar Hover | `#1E2640` | Sidebar category item hover background |

**Color rules:**
1. Every background, accent, badge, and overlay value on every page is one of these values.
2. No color outside this named palette appears anywhere.

### Animated Components

- **DotField background:** install with `npx shadcn@latest add "https://reactbits.dev/r/DotField"`. Place it as a fixed position background layer covering the full viewport, behind all page content. Content sits on top with readable backgrounds.
- **AsciiText logo:** install with `npx shadcn@latest add "https://reactbits.dev/r/AsciiText"`. It replaces the static header logo and renders "UHZMI GAMES" in white or the accent color.

### Button and Interaction States

- Buttons (hover): background shifts to the accent color or brightens, text inverts to white, 150ms ease.
- Buttons (active or press): scale down to 0.97 or 0.98, opacity dip to 0.9, 100ms.
- Buttons (focus): visible focus ring in the accent color with 2px outline offset, required for keyboard accessibility.
- Nav links (hover): text color shifts to the accent color, 150ms ease.
- Sidebar category items (hover): background shifts to #1E2640, slight padding or indent change, 150ms ease.
- Sidebar category items (active): accent color left border or full background highlight.
- Game cards: full hover behavior as described under Game Card Hover States.
- Search input (focus): border color shifts to the accent color with a subtle glow.

---

## Technical Requirements

- **Engine / Framework:** React 18 with Vite. Tailwind CSS for styling.
- **Local backend:** Node.js with Express, minimal, admin panel only, in server.js.
- **Language:** JavaScript and JSX, JSON for data.
- **Platform / Target:** localhost single page application, a current desktop browser, a current mobile browser, responsive.
- **Storage:** local JSON files only. No database. localStorage only for the background music toggle preference.
- **Package manager:** npm. Dev server on localhost:5173.
- **Code quality:** a folder structure matching the layout below, a single dataService.js for all data reads, and a useDebounce.js hook.

### Allowed Tech Stack

1. React 18 with Vite.
2. Tailwind CSS.
3. Node.js with Express for the admin panel only.
4. reactbits.dev DotField and AsciiText components.
5. Lucide React icons (ISC license).
6. Inter font from Google Fonts (SIL Open Font License).
7. Free license itch.io HTML5 games (MIT, GPL, CC0, or free to use).
8. Free license audio from Freesound.org or Mixkit.co (CC0 or free).

### Not Allowed

1. User accounts, registration, login, or authentication of any kind.
2. A database (MySQL, PostgreSQL, Firebase, Supabase, or any other).
3. Comments, ratings, likes, favorites, or any social features.
4. Push notifications, email notifications, or admin dashboard analytics.
5. Video uploads or video content.
6. Payment processing, subscriptions, or any monetization features.
7. iOS or Android mobile app versions.
8. A public production deployment or hosting setup.
9. SEO metadata, sitemaps, or search engine optimization.
10. Third party ads or ad integration.
11. Uploading game files through the admin panel (the admin panel edits JSON only; game files are added manually via the file system).
12. Any backend CMS, WordPress, or database driven content management system.
13. Flash or Ruffle emulation for legacy SWF games.

---

## Design Direction

**Do:**
- Use the exact hex palette for every background, accent, badge, and overlay.
- Keep the page background at #0A0E1A behind the DotField animation.
- Use Inter for all text, with the weights and sizes in the typography table.
- Render the AsciiText logo as "UHZMI GAMES" and the DotField as a fixed full viewport background.
- Use the provided JSON content and footer content exactly as written.

**Do not:**
- Introduce any color outside the named palette.
- Replace Inter with another font.
- Modify the provided categories.json, sounds.json, or footer content.
- Add any feature listed under Not Allowed.

---

## Reference Materials

| Asset | File / URL |
|---|---|
| Layout Reference | `/data/reference` |
| DotField component | `npx shadcn@latest add "https://reactbits.dev/r/DotField"` |
| AsciiText component | `npx shadcn@latest add "https://reactbits.dev/r/AsciiText"` |
| Games source | itch.io free license HTML5 games |
| Cover images source | the itch.io page of each integrated game |
| Sound effect source | Freesound.org (CC0) for click.mp3 |
| Background music source | Mixkit.co (free license) for bgm.mp3 |
| Font | Inter, Google Fonts, SIL Open Font License |
| Icons | Lucide React, ISC License |

**How to use these references:** Match the layout, palette, and typography from the layout reference. Install the DotField and AsciiText components from reactbits.dev. Source the twelve games and their covers from itch.io, and the two sound files from Freesound.org and Mixkit.co, recording every source URL and license in the README.

---

## Deliverables

| # | Item | Format | Notes |
|---|---|---|---|
| 1 | Source archive | `.zip` | Named uhzmi-games.zip, the full project folder ready to extract and run |
| 2 | README.md | `.md` | Setup, JSON schema, "Adding a New Game" covering Method A and Method B, troubleshooting, and license attributions |
| 3 | games.json | `.json` | Populated with all 12 game entries using the schema |
| 4 | categories.json | `.json` | The 12 categories exactly as specified |
| 5 | sounds.json | `.json` | Audio file mappings exactly as specified |
| 6 | /public/covers/ | folder | 12 cover images, 640x360 JPG, sourced from itch.io game pages |
| 7 | /public/sounds/ | folder | 2 free license MP3 files: click.mp3, bgm.mp3 |
| 8 | /games/ | folder | 12 game folders, each containing a playable index.html |
| 9 | server.js | `.js` | Minimal Express server for admin panel writes |
| 10 | Source code | React | All components, pages, services, and hooks per the folder structure |

### File Naming Convention

The source archive uses the exact name uhzmi-games.zip. The setup file uses the exact name README.md. Game folder names and cover file names use the game slug: lowercase letters with hyphens between words and no spaces. Cover files are JPG named [slug].jpg. Game folders are /games/[slug]/ with index.html at the root.

```
lowercase-with-hyphens
```

Rules:
- Use lowercase letters.
- Use a hyphen between words.
- No spaces.

### Folder Structure (deliver exactly, no deviations)

```
uhzmi-games/
├── public/
│   ├── covers/            <- all game cover images (640x360 JPG, named by slug)
│   └── sounds/            <- free license audio files (click.mp3, bgm.mp3)
├── src/
│   ├── components/
│   │   ├── Header.jsx
│   │   ├── Sidebar.jsx
│   │   ├── Footer.jsx
│   │   ├── GameCard.jsx
│   │   ├── GameGrid.jsx
│   │   ├── SearchBar.jsx
│   │   ├── TopFiveCarousel.jsx
│   │   ├── CategoryRow.jsx
│   │   └── BackgroundMusic.jsx
│   ├── pages/
│   │   ├── HomePage.jsx
│   │   ├── CategoryPage.jsx
│   │   ├── GamePage.jsx
│   │   ├── SearchResultsPage.jsx
│   │   └── AdminPage.jsx
│   ├── data/
│   │   ├── games.json
│   │   ├── categories.json
│   │   └── sounds.json
│   ├── services/
│   │   └── dataService.js   <- single file for all data reads
│   ├── hooks/
│   │   └── useDebounce.js
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
├── games/                   <- individual game folders, each with index.html
├── server.js                <- minimal Express server for admin panel
├── package.json
├── tailwind.config.js
├── vite.config.js
├── README.md
└── .gitignore
```

---

## Build / Export Specifications

- **Build:** a .zip archive named uhzmi-games.zip holding the full project folder, ready to extract and run.
- **Start commands:** npm install installs all dependencies, npm run dev starts the dev server on localhost:5173.
- **Backend:** the Express server for the admin panel starts alongside Vite or is reachable through Vite proxy configuration.
- **Final setup:** requires only npm install && npm run dev with no manual server configuration.

---

## Scope Boundaries

### DO

1. A fully working React and Vite website that runs with npm run dev on localhost.
2. All pages: Homepage, Category pages, Game play page, Search results page, Admin page.
3. Static footer pages: About, FAQ, Terms of Use, Privacy Policy, Contact, using the provided content.
4. A dark themed UI with the exact color palette.
5. The DotField animated background across the entire site.
6. The AsciiText animated "UHZMI GAMES" logo in the header.
7. A left sidebar with all 12 categories from categories.json.
8. Game cards with all hover effects.
9. A search bar with a live autocomplete dropdown.
10. The Top 5 Most Played carousel on the homepage.
11. Category rows with horizontal carousels and "See all" links.
12. A game play page with iframe embedding from the local /games/ folder.
13. The play count increment system via the local Express server.
14. Category pages with sort and filter: Most Popular, Newest First, Oldest First, A to Z, Z to A.
15. Tag based filtering.
16. Responsive design: a mobile hamburger sidebar and a grid that reflows to 2 columns.
17. 12 itch.io games fully integrated into games.json.
18. Cover images for all 12 games in /public/covers/.
19. Two free license sound files sourced and integrated.
20. A background music toggle with localStorage persistence.
21. A card click sound effect.
22. A minimal admin panel at /admin with Add, Edit, and Delete.
23. An Express server in server.js to handle admin form submissions writing to games.json.
24. A dataService.js abstraction layer for all data reads.
25. A folder structure matching the layout exactly.
26. A README.md with setup, JSON schema reference, and an "Adding a New Game" section covering both methods.
27. Licenses and resources documented in the README.

### DO NOT

1. No visitor accounts, login flow, or sign up flow.
2. No database of any kind.
3. No comments, ratings, likes, favorites, or social features.
4. No push notifications, email notifications, or analytics dashboards.
5. No video uploads or video content.
6. No payment flow, subscriptions, or monetization.
7. No native iOS or Android application.
8. No public production deployment or hosting setup.
9. No SEO metadata, sitemaps, or search engine optimization.
10. No third party ads or tracking scripts.
11. No uploading of game files through the admin panel.
12. No backend CMS, WordPress, or database driven content management.
13. No Flash or Ruffle emulation for legacy SWF games.

---

## Tool Requirements

- **Required tools:** any code editor. npm and Node.js installed locally.
- **Runtime:** a current desktop browser and a current mobile browser.
- **Forbidden:** any paid library, any database, and any backend beyond the minimal Express admin server.

---

## Quality Control / Pre-Submission Checklist

Before submitting, confirm all of the following:

1. [ ] npm install and then npm run dev start the site on localhost with zero errors.
2. [ ] All 12 game cards appear on the homepage with correct covers, titles, and categories.
3. [ ] Every background, accent, badge, and overlay value matches the named hex palette.
4. [ ] All text uses Inter with the specified weights and sizes.
5. [ ] The header logo renders UHZMI GAMES and the DotField background is fixed behind content.
6. [ ] categories.json, sounds.json, and the footer content match the PRD exactly.
7. [ ] games.json holds all 12 entries with every field filled.
8. [ ] The folder structure matches the layout exactly.
9. [ ] No errors appear in the browser console on any page.
10. [ ] The site is responsive: a 2 column grid and a hamburger sidebar on mobile.

---

## Acceptance Checklist

The delivery is complete only if every item passes.

1. [ ] npm install and npm run dev start the site on localhost with zero errors.
2. [ ] All 12 game cards appear on the homepage with correct covers, titles, and category tags.
3. [ ] Hovering any card triggers the full animation: scale up, shadow, overlay, play icon.
4. [ ] Clicking a category in the sidebar filters the grid to only that category.
5. [ ] All 5 sort options work on category pages: Most Popular, Newest, Oldest, A to Z, Z to A.
6. [ ] Searching for a game title shows it in the autocomplete dropdown.
7. [ ] Clicking a game card opens the game page and the game loads inside the iframe.
8. [ ] The play count increments and the Top 5 section reflects the most played games.
9. [ ] The admin panel at /admin allows adding a new game that appears on the site.
10. [ ] The admin panel allows editing an existing game entry.
11. [ ] The admin panel allows deleting a game entry, which removes the card from the site.
12. [ ] The background music toggle works and the preference survives a page refresh.
13. [ ] The card click sound plays when clicking a game card.
14. [ ] The site is fully responsive and works on mobile viewport widths.
15. [ ] All 5 footer links open their content pages or modals.
16. [ ] The README contains all required sections with clear instructions.

---

## Evaluation Criteria

The project will be evaluated against the following points:

- Every background, accent, badge, and overlay value is one of the named hex values.
- The homepage shows all 12 games, with the Top 5 Most Played carousel and one row per category.
- Game card hover runs the full animation sequence and reverses smoothly with no instant snap.
- Search autocomplete returns matching titles with thumbnails.
- Each game loads in the iframe on its game page, and the play count increments on start.
- The admin panel adds, edits, and deletes games, writing to games.json through the Express server.
- The background music toggle persists in localStorage and the card click sound plays.
- The site is responsive with a 2 column mobile grid and a hamburger sidebar.
- The README documents setup, the JSON schema, both add methods, troubleshooting, and all license attributions.

---

## Developer's Choices

| Decision | Accepted Options |
|---|---|
| Which 12 itch.io games | Any free license (MIT, GPL, CC0, or free to use) HTML5 games matching the 12 category specs; substitutions need owner approval |
| Cover image crop | Any crop or resize that yields a 640x360 JPG |
| Sound files | Any CC0 or free license click sound and background music within the stated lengths and sources |
| Load More vs infinite scroll | Either option on category pages |
| Admin panel styling | Functional UI is sufficient |
| Spacing where no value is fixed | Worker judgment |

---

## Delivery Terms

- **Delivery method:** a .zip archive named uhzmi-games.zip containing the full project folder.
- **Acceptance:** governed by the Acceptance Checklist above. Every item must pass.
- **Revisions:** to be agreed with the project owner.
- **Allowed revision types:** palette values, layout values, font values, game wiring, and admin panel behavior.
- **What does not count as a revision:** a full redesign or an expansion of scope beyond this brief.

---

## Final Goal

Success is a dark themed React and Vite portal that runs offline on localhost with npm run dev, where a visitor browses game cards by category, sees the Top 5 Most Played, searches with live autocomplete, sorts and filters a category, opens a game page, and plays one of twelve self hosted itch.io HTML5 games inside an iframe with the play count incrementing. The owner can add, edit, and delete games through the minimal admin panel at /admin, which writes to games.json through the Express server. The site uses only the named hex palette and Inter typography, includes the DotField background and the AsciiText logo, plays the card click sound and the toggleable background music, and ships as uhzmi-games.zip with a complete README covering setup, the JSON schema, both methods of adding a game, troubleshooting, and license attributions.
