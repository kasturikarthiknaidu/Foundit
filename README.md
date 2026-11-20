# FoundIt - Campus Lost & Found Platform Prototype

FoundIt is a responsive campus lost-and-found web application built for college campuses to centralize lost property reports, automate item matching between lost and found entries, and manage confidential ownership verification claims.

## 📁 Project Architecture & Files

```
foundit-prototype/
├── index.html              # Main HTML5 application shell & view sections
├── css/
│   └── styles.css          # Mobile-first CSS Grid styles & responsive media queries
├── js/
│   ├── api.js              # Mock REST Fetch API client & local data store
│   └── app.js              # UI controller, debounced search, modal & matcher scripts
├── src/
│   └── types.ts            # TypeScript data model contracts & interfaces
└── README.md               # Setup and architecture documentation
```

## 🚀 Module Breakdown

### Modules 1–2: Static Phase (HTML/CSS & Guidelines Hub)
* **CSS Grid Showcase**: Mobile-first media queries (`@media (min-width: 640px)` for tablet, `@media (min-width: 1024px)` for desktop) rendering flexible 1, 2, and 3-column card layouts.
* **Status Badges & Item Cards**: Custom CSS pills (`Open`, `Claim Pending`, `Resolved`), category tags, and responsive SVG/photo containers.
* **Guidelines & Policy Hub**: Campus recovery protocols and security desk custody office contact table.

### Modules 3–4: Dynamic Phase (TypeScript/JS & Claim Workflow)
* **Typed Data Contracts (`types.ts`)**: Strongly typed interfaces for `LostFoundItem`, `ClaimRequest`, `MatchResult`, `CampusLocation`, and `ItemCategory`.
* **Item Reporting Console**: Interactive submission form for Lost or Found property with real-time state persistence.
* **Automated Item Matching Engine**: Cross-references Lost vs Found items based on category, campus location zone, date, and keyword similarity with confidence score calculation (e.g. 88% Match Confidence).
* **Secure Ownership Claim Modal**: Confidential claim modal requiring claimants to answer private identifying proof (wallpaper, serial numbers, lock codes) before releasing items.

## 🛠️ How to Run
Simply open `index.html` in any modern web browser. No external server setup or node dependencies required to run the prototype demo!
