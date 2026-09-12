# Changelog

## 0.1.0-beta.1

Initial beta release.

- Registers DeepSeek Harness as a Paseo provider with the public ACP shim.
- Launches the official DSH ACP profile without a shell.
- Bridges DSH session/resume to the shim private session/load expectation
  only when the initialized peer advertises resume but not load.
- Preserves DSH model, reasoning, MCP, image, tool, usage, permission and
  cancellation behavior without local session or credential storage.
- Supports and tests DSH 0.1.5-rc.1 and 0.1.5-rc.2.
- Closes connector resources during version probing, initialization and active
  prompts without allowing a post-close ACP child spawn.
- Records separate live public-SDK verification for both CLI versions; see the
  README for the exact scope and desktop/mobile limitations.
