This project is a Vite React TypeScript application for analyzing public GitHub profiles through the GitHub REST API.

Architecture:
- `src/main.tsx` mounts the React app, React Router routes, and the global context provider.
- `src/pages/HomePage.tsx` coordinates profile searches, URL-driven usernames, comparison loading, and PDF export.
- `src/components/` contains focused UI components for search, profile details, stats, charts, repository browsing, and application states.
- `src/services/github.ts` is the only module that calls the GitHub REST API. Keep API response shaping and derived profile metrics there.
- `src/context/AppContext.tsx` owns dark/light theme, recent searches, and favorites. These are browser-local preferences stored in Local Storage.
- `src/types/github.ts` defines shared GitHub and analyzer data types.
- `src/utils/format.ts` contains display formatting helpers.

Conventions:
- Use React hooks and functional components.
- Keep data fetching out of presentational components when practical.
- Prefer existing Tailwind component classes in `src/styles.css` for consistent glassmorphism panels, buttons, inputs, and cards.
- Do not introduce server persistence for recent searches or favorites unless the product requirements change; they are intentionally local to each browser.
- The app is static and deploys from `dist` after `npm run build`.

Deployment:
- Netlify uses `netlify.toml`.
- Vercel uses `vercel.json` with SPA rewrites to `index.html`.
