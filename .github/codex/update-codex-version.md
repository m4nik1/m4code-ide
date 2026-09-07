The workflow has updated the exact `@openai/codex` dependencies in
`packages/codex-protocol/package.json` and `apps/novus/package.json` to the
latest published version.

Regenerate and verify the protocol by running:

1. `npm run generate -w @lightcode/codex-protocol`
2. `npm run protocol:check -w @lightcode/codex-protocol`
3. `npm run typecheck -w @lightcode/codex-protocol`
4. `npm test -w @lightcode/codex-protocol`

Inspect any failures and make only the changes required for compatibility with
the updated Codex version. Do not change the selected Codex version. Do not
commit, push, or create a pull request; the workflow handles those operations
after this step.
