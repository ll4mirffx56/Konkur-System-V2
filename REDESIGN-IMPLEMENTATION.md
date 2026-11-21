# Moroor V2 — Cyber-Academic UI refresh

This package applies a substantial visual-system refresh to the existing Moroor V2 application while preserving its existing React behavior and data contracts.

## UI changes
- Reworked the visual language around an obsidian workspace, restrained indigo/cyan accents, layered translucent panels, and finer borders.
- Updated sidebar, navigation states, workspace header, stat cards, charts, goal ring, review list, quick actions, authentication surface, focus states, and hover/motion behavior.
- Added responsive tablet/mobile treatment: compact horizontal navigation, sticky workspace header on desktop, reduced mobile header controls, and two-column metric cards.
- Added reduced-motion handling and retained the light theme with a coordinated palette.

## Deliberately unchanged
- `src/logic.ts`
- `src/goalExam.ts`
- `src/cloudSync.ts`
- `src/cloud.ts`, Supabase authentication, compare-and-swap writes, Realtime subscriptions, and data hydration flow
- Jalali conversion/date entry behavior and timezone handling
- Test percentage formula, review intervals, import/export and user data structures
- GitHub Pages Vite base-path detection and deployment workflow

## Validation
- `npm test`: 49 tests passed.
- Production `npm run build` was not run in this environment because dependency installation could not complete. GitHub Actions must complete the production build before the updated site is considered deployed.
