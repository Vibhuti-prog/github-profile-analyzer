# GitHub Profile Analyzer

A modern GitHub Profile Analyzer built with React, Vite, TypeScript, Tailwind CSS, React Router, Axios, Framer Motion, Recharts, and the GitHub REST API.

## Features

- Search any public GitHub username.
- Display avatar, name, username, bio, location, company, blog, followers, following, repositories, gists, and account creation date.
- Show top repositories sorted by stars.
- Search, filter, and sort repositories by stars, forks, or last updated date.
- Display stars, forks, language, and last updated date for repositories.
- Show activity-oriented contribution statistics based on public repository update data.
- Render a language usage chart with Recharts.
- Compare two GitHub profiles side by side.
- Save favorite profiles and recently searched profiles in Local Storage.
- Copy, share, and download profile information as a PDF.
- Toggle dark and light themes.
- Responsive glassmorphism UI with smooth Framer Motion animations.
- Error, loading, empty, and user-not-found states.

## Tech Stack

- React 19
- Vite 7
- TypeScript
- Tailwind CSS 4
- React Router
- Axios
- Context API
- Framer Motion
- Recharts
- jsPDF and html2canvas
- ESLint and Prettier

## Getting Started

Install dependencies:

```bash
npm install
```

Run locally:

```bash
npm run dev
```

Create a production build:

```bash
npm run build
```

Run linting:

```bash
npm run lint
```

Format files:

```bash
npm run format
```

## Deployment

### Vercel

The project includes `vercel.json` configured for Vite:

- Build command: `npm run build`
- Output directory: `dist`
- SPA rewrites to `index.html`

Import the repository in Vercel and keep the detected Vite settings, or use the included config.

### Netlify

The project includes `netlify.toml`:

- Build command: `vite build`
- Publish directory: `dist`

## Notes

The GitHub REST API works without a token for public data but is subject to unauthenticated rate limits. The app only stores favorites, theme, and recent searches in the browser's Local Storage.

# Live Demo
http://magical-tanuki-d4538a.netlify.app

# Future Improvements

- GitHub OAuth
- Contribution Heatmap
- AI Profile Analysis
- Repository Insights
- Export as PNG

#  Author

Vibhuti

GitHub: https://github.com/Vibhuti-prog

LinkedIn: https://www.linkedin.com/in/vibhuti2005/

