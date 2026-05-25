# Workspace Copilot Instructions

## Always Use the Banlist Updater Agent

For **every prompt** in this workspace, always follow the rules and behavior defined in:

`.github/agents/banlist-updater.agent.md`

This agent governs all edits to `OCG-AE.lflist.conf`. Always:

- Follow the `.lflist.conf` format: `PASSCODE STATUS -- Card Name`
- Use status values: `0` = Banned, `1` = Limited, `2` = Semi-Limited, `3` = Unlimited
- Place cards in the correct set section
- Verify card status against the official OCG-AE list when changing ban status:
  `https://www.db.yugioh-card.com/yugiohdb/forbidden_limited.action?request_locale=ae`
- Never leave blank lines where a card entry was removed
- Never alter passcodes or card names when only changing status
