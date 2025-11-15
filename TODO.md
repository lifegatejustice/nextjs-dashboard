# TODO: Fix Vercel Deployment Issue with bcrypt

- [x] Update package.json: Replace "bcrypt": "^6.0.0" with "bcryptjs": "^2.4.3" in dependencies
- [x] Update package.json: Remove "bcrypt" from "onlyBuiltDependencies" array
- [x] Update auth.ts: Change import from 'bcrypt' to 'bcryptjs'
- [x] Update app/seed/route.ts: Change import from 'bcrypt' to 'bcryptjs'
- [x] Run pnpm install to update lockfile
- [x] Remove deprecated @types/bcryptjs (bcryptjs has built-in types)
- [x] Create types.d.ts for bcryptjs TypeScript declarations
- [x] Add export const dynamic = 'force-dynamic' to create/page.tsx
- [x] Update all database connections to use DATABASE_URL || POSTGRES_URL
- [ ] Test build locally to ensure no errors
