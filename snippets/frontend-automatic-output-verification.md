## Dev Server & Manual Verification

- **NEVER** start the dev server (`yarn dev`, `next dev`, etc.) yourself.
- **NEVER** make requests (curl, fetch, browser automation) to the dev server (`localhost:3000` or similar) to check output.
- The user runs and verifies the app themselves. After implementing a change, state that implementation is done and provide clear manual verification steps (what to click/hover, what to expect) instead of checking it yourself.
