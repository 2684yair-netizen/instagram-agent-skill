# Yairlines Instagram workspace

The 13 Instagram skills live in `.claude/skills/ig-*` and load automatically in
any session opened on this repo.

- Always answer the user in Hebrew. Everything written for Instagram (scripts,
  on-screen text, captions, stories, comments, DMs) is in Hebrew unless asked
  otherwise.
- The skills' memory lives in `instagram/` (not `~/.claude/instagram/`):
  `voice.md`, `log.md`, `swipe.md`, `plan.md`. Read `instagram/voice.md` before
  writing anything. This container is wiped when the session ends, so after
  changing anything in `instagram/`, commit and push it.
- Run the Python tools from the repo root, e.g.
  `python3 .claude/skills/ig-reel/hookscore.py --hook "..."`.
- The hook scorer, beat timer, caption linter and humanizer were tuned on
  English. On Hebrew text treat their scores as rough; the skills' written
  guidance still applies.
- Nothing gets posted. Every skill ends with a copy-ready block the user posts.
