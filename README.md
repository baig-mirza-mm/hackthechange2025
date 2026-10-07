# Fix It Calgary

## Overview
Fix It Calgary is a web-based, issue reporting platform built during **Hack the Change 2025**. The application allows users to pin locations on a map and write reports describing issues they encounter in specific areas, enabling awareness of community concerns.

The project was designed and built within a 24-hour window, prioritizing rapid prototyping, core functionality, and usability under tight time constraints.

## Features
- Interactive map for selecting and pinning locations
- User-submitted issue reports with written descriptions
- Location-based display of reported issues
- Simple, responsive user interface designed for fast iteration

## Tech Stack
- **Frontend:** React, Vite
- **Styling:** Tailwind CSS
- **Hosting / Deployment:** AWS

## Run Locally

### Requirements
- Node.js 20.19 or newer, or 22.12 or newer
- npm

### Setup
```sh
npm ci
npm run dev
```

Vite prints the local URL when the development server starts (usually
`http://localhost:5173`). Open that URL in a browser. The landing page is at `/`,
and the map/report view is at `/home`.

The `/home` view loads and creates issues through the backend configured in
`src/pages/Home.tsx`. That API must be reachable for issue data and submission
to work; the landing page can run without it.

### Other Commands
```sh
npm run build    # Create a production build in dist/
npm run preview  # Serve the production build locally
npm run lint     # Run ESLint
```

![Front page](assets/screenshots/front-page.png)
![Map view showing pinned issues](assets/screenshots/map-view.png)
