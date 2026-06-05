@[assistant]:
Fixed in [src/index.js](/public-demo/run-workspace/repo/src/index.js:283): `YYYY` now uses the existing `Utils.s(..., 4, '0')` pad helper, so years like `1` format as `0001`.

Validation passed:

```bash
npx jest test/display.test.js --runInBand --coverage=false
```

Result: `31 passed`. Note: existing untracked files remain untouched: `AGENTS.md`, `CLAUDE.md`, and an `.npm-cache` log.