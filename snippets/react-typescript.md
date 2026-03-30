### Code Style & Linting
- **Filenames**: kebab-case enforced by ESLint (`filename-rules/match`)
- **No console.***: Use `logger` from `src/logger.ts` instead (ESLint error)
- **No `any` type**: NEVER use `any` in TypeScript. If working with an API object whose types don't seem to exist yet, do NOT fall back to `any` — instead, stop and inform the user to run `yarn swagger:codegen` to generate the missing API types from the Swagger spec.
- **TypeScript strict mode**: enabled with `noUncheckedIndexedAccess`
- **Import paths**: Use `@/*` alias for `src/*`
- Pre-commit hooks run `yarn typecheck` and `yarn lint-staged`
- Single quotes for strings, semicolons required
- **Hook ordering in components**: Place `useEffect` calls right before the first `return` statement of a React component. All other hooks (`useState`, `useMemo`, `useCallback`, queries, etc.) should come first, followed by handler functions, then `useEffect` calls, then `return`.
