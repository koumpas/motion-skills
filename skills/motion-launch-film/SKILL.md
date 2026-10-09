---
name: motion-launch-film
description: "Direct short product launch films and brand motion. Use for a launch video, feature reveal, product promo, or brand sting that needs a concept and an editable composition. For an isolated animation edit or a critique, use the corresponding task guidance instead."
metadata:
  version: "0.1.0"
---

# Product launch motion

Make the viewer understand one product change through a visible event.
Keep the source editable so the user can revise copy, assets, format, and motion.

## Scope and tools

Respect the requested length, format, assets, and approval state.
Do not expand a simple edit into a new launch film.
In fal Agent, activate the existing `video-compositing` skill before composition code.
It owns the sandbox, renderer, asset paths, render budget, and delivery workflow.
In another agent, use its installed composition workflow and documented renderer.
If no renderer is available, deliver the concept and plan, and state the production dependency.
Do not claim a rendered video from a plan or source code alone.
Generate missing media with available tools when the brief requires it.
Use editable text and geometry for controlled animation, typography, and product UI.

If `motion-choreography` or `motion-review` is available, activate it for the corresponding phase.
If either is absent, apply the motion and review requirements below directly.
These companion skills are optional; do not invent unavailable tool calls.

## Establish the product change

Extract these facts from the brief and available brand material:

- The viewer and the intended response.
- One product action, its visible result, and the evidence available to show it.
- The supplied logo, typeface, colors, imagery, UI, and copy.
- The requested duration, format, audio, and deliverables.

Use real screens and product outputs where available.
Declare illustrative demo content in the delivery note.
Do not present invented results, customers, statistics, or features as product evidence.
If one missing fact changes the concept, ask for it while inspecting the available assets.
Otherwise state a brief assumption and proceed.

## Choose a concept

For a new film, compare up to three materially different concepts before selecting one.
A simple brand sting may need only one clear concept.
Prefer an idea where the product's action determines the motion.
For example, a selection can become a crop; a search can reveal a result; a merge can join two paths.
These are mechanics to consider, not default scenes to repeat.

Judge concepts by clarity, brand fit, available evidence, and production cost.
Reject a concept that requires an unsupported product claim or an unreadable demonstration.
Keep the selection rationale short. Show alternatives only when they help the user's decision.
Do not introduce a new approval gate when the user already authorized production.

## Plan the film

For a film with several scenes, write a compact `MOTION_PLAN.md` in the project.
Use [references/film-plan.md](references/film-plan.md) for the plan and worked example.
For a single sting, record the same decisions in a short project note.

Choose one visual system: type hierarchy, color meanings, material, light, and camera behavior.
Make each beat either explain the product change or connect necessary context.
Remove a beat whose deletion preserves the message and its evidence.
Name the main subject in each shot. Other elements should support that subject.
Give transitions a reason: continue an action, reveal a result, change context, or mark completion.
A clean cut is valid. A carried object is optional.

Brand guidance and the explicit brief control visual choices.
Use these task-specific design criteria before generic house-style defaults.
Retain the renderer's technical and determinism requirements.
Do not add grain, glow, lines, UI chrome, or 3D solely to fill empty space.
Use an effect when it helps the product action or the intended character of the film.

## Build and inspect

Build the hardest product action and transition first.
Inspect its start, intermediate state, result, and transition boundary.
If it fails to communicate the product change, revise that beat before building the rest.

For motion, record the start state, end state, duration, curve, and overlap.
Make acceleration serve the action. Give text enough time to read at the final output size.
Use different parent and child layers for concurrent motions that need separate controls.
Keep all animation on the renderer's frame clock.

Render a draft through the existing production workflow.
Inspect representative frames and frames around important transitions.
Inspect playback when a playback tool is available.
Check audio separately when the film includes audio.
Repair broken assets, product inaccuracies, unreadable proof, and discontinuities before cosmetic finish.
Report inspection limits instead of claiming checks that did not occur.

## Deliver and preserve

Deliver the requested video through the available production workflow.
In fal Agent, use its existing output and delivery tools.
Keep the composition, assets, and plan in the project for subsequent edits.
Do not claim that sandbox files are durable storage.
Expose an editable-source package only when the user requests one or the environment supports it.
In the delivery note, state the concept, checked behavior, illustrative content, and unresolved limits.
For a revision, preserve approved elements and compare the changed region with the previous draft.
