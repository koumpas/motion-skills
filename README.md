# Motion Skills

**Product launch direction, motion choreography, and render review.**

Start with a product action and its visible result. Use motion to make that result clear. Preserve approved work during a revision.

## Install

```bash
npx skills add koumpas/motion-skills
```

Choose the skills and target agent when prompted. To install one skill:

```bash
npx skills add koumpas/motion-skills --skill motion-launch-film
```

To install all three in a Codex project:

```bash
npx skills add koumpas/motion-skills --skill '*' --agent codex
```

For SSH access:

```bash
npx skills add git@github.com:koumpas/motion-skills.git
```

The [skills CLI](https://github.com/vercel-labs/skills) installs these folders. This repository requires no separate npm package.

## Choose a skill

| Skill | Purpose | Example request |
|---|---|---|
| [motion-launch-film](skills/motion-launch-film/SKILL.md) | Choose a concept, plan a film, and direct production | Create a silent 10-second feature reveal from these product screens. |
| [motion-choreography](skills/motion-choreography/SKILL.md) | Design typography, object motion, camera moves, and transitions | Change the CTA and preserve the other copy and motion. |
| [motion-review](skills/motion-review/SKILL.md) | Inspect a render, report defects, and complete authorized repairs | Review this video with timestamped findings. Keep the source unchanged. |

The skills work separately. Companion skills are optional.

## Production requirements

These are design instructions. They contain no renderer, media models, fonts, or executable scripts.

In fal Agent, enable its existing `video-compositing` skill. That workflow handles composition, assets, rendering, and delivery.

Other agents need an installed composition and rendering workflow to produce video. The skills can guide a concept, choreography, or review with the available tools. Installation alone does not provide video production tools.

## Import into fal Agent

Import each folder through fal Agent's GitHub skill import interface:

- [motion-launch-film](https://github.com/koumpas/motion-skills/tree/main/skills/motion-launch-film)
- [motion-choreography](https://github.com/koumpas/motion-skills/tree/main/skills/motion-choreography)
- [motion-review](https://github.com/koumpas/motion-skills/tree/main/skills/motion-review)

Use a folder link for each skill. Enable `video-compositing` alongside the imported skills. The local `npx` command does not import skills into a hosted fal Agent account.

## Try it

Supply verified product screens, brand assets, and a brief. For example:

```text
Use motion-launch-film to create a silent 10-second launch film.
Show one real product action and its visible result from the supplied assets.
Use editable text and geometry for precise motion.
Keep the source project for a later revision.
Deliver the video and state which checks you completed.
```

Then request a precise revision:

```text
Use motion-choreography on the previous source project.
Change the CTA to "Start with one idea."
Preserve the footage, palette, other copy, shot order, camera movement,
and transition timing. Make the smallest necessary layout change.
```

## Status and validation

Version 0.1.0 is an early release. See [practical trials](evaluation.md) for a complete film, a narrow revision, and a critique.

Distribution checks passed with `skills` version 1.7.1:

- The CLI found all three skills.
- The public repo installed in a temporary Codex project.
- The installed skill files and plan reference matched the source.
- fal's GitHub importer read all three public folder links without warnings.

These checks do not prove video quality or runtime compatibility. No controlled video-quality comparison or hosted fal Agent account import occurred for this release.

## License

[MIT license](LICENSE).
