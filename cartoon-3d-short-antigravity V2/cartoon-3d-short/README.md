# Cartoon 3D Short (Universal Agent Skill)

A portable Agent Skill package based on the MIT-licensed [`mromidev/claude-animated-shorts`](https://github.com/mromidev/claude-animated-shorts) project. It guides an AI coding agent through producing ~55–70 second vertical animated story shorts: flat 2D cartoon characters inside colourful 3D toon environments, rendered with Three.js and Remotion, with narration, synthesized sound effects, and an original score.

The original workflow and project assets are retained. The skill instructions have small portability edits so they do not assume Claude-only tools; the same `SKILL.md` can be used by compatible skill hosts such as Claude Code, OpenAI Codex, and Google Antigravity.

## Install

Unzip the archive. Copy the folder `cartoon-3d-short` (the folder containing `SKILL.md`) into the skill directory for your agent:

| Agent | Global skill directory | Project/workspace directory |
|---|---|---|
| Claude Code | `~/.claude/skills/cartoon-3d-short/` | `.claude/skills/cartoon-3d-short/` |
| OpenAI Codex | `~/.agents/skills/cartoon-3d-short/` | `.agents/skills/cartoon-3d-short/` |
| Google Antigravity | `~/.gemini/config/skills/cartoon-3d-short/` | `.agents/skills/cartoon-3d-short/` |
| Other Agent Skills-compatible agents | Use that agent's documented skills directory | Use that agent's documented project skills directory |

Restart/reload the agent or its skills list if the new skill does not appear. Then prompt it with something like:

> Use the `cartoon-3d-short` skill and make a short about [your topic].

## Requirements

This package is the workflow and templates, not a prebuilt renderer. The machine/project still needs Node.js, Python 3, FFmpeg, Remotion, `@remotion/three`, and the dependencies used by the templates. See `SKILL.md` for the full pipeline and render commands.

## Package contents

- `SKILL.md` — workflow instructions and portable agent guidance.
- `templates/bridge/` — complete example Three.js/Remotion composition source.
- `templates/audio/` — audio synthesis and mixing helpers.
- `templates/scripts/` — still rendering, sheet generation, merging, and QA helpers.
- `references/` — style bible, measurement reports, and visual reference material.

## Important notes

- Create original stories, characters, narration, and shots. Do not copy third-party scripts, characters, or shot sequences.
- The bundled reference frames and sheets are included for private style study only. Do not upload, publish, or send those reference videos/images to third parties.
- Keep the copyright and license notices when copying or redistributing the code and documentation. See `LICENSE`.

## Credits

Based on **Claude Animated Shorts** by mromidev. The original project is licensed under the MIT License; see `LICENSE` for the full notice.
