# oh-my-claudecode v5.7.13: More reliable keyword prompts and team handling

## Release Notes

This release preserves explicit keyword invocations in reference prompts, keeps help requests informational across more prompt shapes, and corrects team and notification environment handling. Thanks to @rudycelekli and @iyoda for their fixes, and to @rolldav for reporting #4550.

### Highlights

- **fix: preserve explicit keyword invocation in reference prompts** (#4551, fixes #4550; reported by @rolldav)
- **fix(keyword-detector): keep leading help requests informational in two more shapes** (#4564)
- **fix(team): point the pane-ready timeout hint at OMC_TEAM_READY_TIMEOUT_MS** (#4568)

### Bug Fixes

- **fix: preserve explicit keyword invocation in reference prompts** (#4551, fixes #4550; reported by @rolldav)
- **fix: resolve #4551 regressions in keyword-detector** (#4553)
- **fix(keyword-detector): keep leading help requests informational in two more shapes** (#4564)
- **fix(notifications): stop truncating OMC_NOTIFY_TMUX_TAIL_LINES** (#4556, @rudycelekli)
- **fix(team-dispatch): stop truncating cooldown environment values** (#4557, @rudycelekli)
- **fix(team): read the start-submit timeout as a whole integer** (#4558, @rudycelekli)
- **fix(team): point the pane-ready timeout hint at OMC_TEAM_READY_TIMEOUT_MS** (#4568, @iyoda)

### Other Changes

- **test: stabilize concurrent workflow-profile stops** (#4561, fixes #4560)
- **ci: authorize generated artifacts during an earlier v5.7.12 main-to-dev sync attempt** (#4563, #4565, #4567)
- **chore(sync): merge the v5.7.12 main release into dev** (#4569)
- **ci: authorize and refresh generated artifacts for the v5.7.12 main-to-dev sync** (#4570, #4573, #4574)

### Stats

- **15 merged PRs** | **7 bug fixes** | **8 other changes**

### Install / Update

The npm CLI and the Claude Code marketplace/plugin are separate install tracks, not either/or replacements. Update whichever track you use; if you have both installed, update both. CLI-dependent skill paths such as `ask` and CLI-backed `team` require the `omc` CLI from the npm package.

**CLI / runtime:**

```bash
npm install -g oh-my-claude-sisyphus@5.7.13
```

**Claude Code plugin:**

```text
/plugin marketplace update omc
```

**Full Changelog**: https://github.com/Yeachan-Heo/oh-my-claudecode/compare/v5.7.12...v5.7.13

## Contributors

Thank you to all contributors who made this release possible!

@iyoda @rudycelekli @Yeachan-Heo
