# AGENTS.md - MamiModa Fashion Starter

## Build/Lint/Test Commands
- **Dev**: `cd fashion-starter/storefront && yarn dev` (runs on port 8000)
- **Build**: `cd fashion-starter/storefront && yarn build`
- **Lint**: `cd fashion-starter/storefront && yarn lint`
- **E2E Tests**: `cd fashion-starter/storefront && yarn test-e2e`
- **Single E2E Test**: `cd fashion-starter/storefront && npx playwright test e2e/tests/path/to/test.spec.ts`

## Code Style Guidelines
- **TypeScript**: Strict mode enabled, use proper typing
- **Imports**: Use path aliases (`@lib/*`, `@modules/*`, `@/components/*`)
- **Formatting**: Prettier config - no semicolons, double quotes, 2 spaces, trailing commas
- **Components**: Use `"use client"` directive for client components, `"use server"` for server actions
- **Naming**: PascalCase for components, camelCase for functions/variables, kebab-case for files
- **File Structure**: Components in `index.tsx`, group by feature in modules
- **Styling**: TailwindCSS with `twMerge` for conditional classes
- **Error Handling**: Use try/catch with proper error messages, validate inputs with zod
- **React**: Use React 19 patterns, proper hooks usage, server/client component separation
- **Exports**: Default exports for components, named exports for utilities

## Project Structure
- Next.js 15 storefront with Medusa 2.0 backend integration
- React 19, TypeScript, TailwindCSS, React Query, Playwright for E2E