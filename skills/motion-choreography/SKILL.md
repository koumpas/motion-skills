---
name: motion-choreography
description: "Design or revise typography, object motion, camera moves, and transitions in an editable launch film or brand animation. Use when the task needs controlled choreography or a precise motion edit. It does not generate unrelated footage."
metadata:
  version: "0.1.0"
---

# Motion choreography

Make motion communicate an action, change, or emphasis.
For each meaningful movement, define what changes and what remains stable.

## Establish the edit boundary

Read the current composition and relevant plan before an edit.
Identify the selected element, affected time interval, and approved properties to preserve.
If the user changes one word, preserve the other copy, assets, timing, and choreography where possible.
If the new text cannot fit or remain readable, explain the smallest necessary layout or timing change.
Do not redesign the film to accommodate a routine edit.

In fal Agent, activate the existing `video-compositing` skill before composition code.
Keep its asset, runtime, render, and delivery requirements.
Use the available renderer's documentation for exact APIs.

## Specify the movement

Record start state, end state, duration, motion curve, and overlap for the important movement.
An easing curve defines how speed changes during the movement.
Choose the curve from the action:

| Action | Useful starting choice | Reason to change it |
|---|---|---|
| An object arrives and settles | Decelerate toward the result | A physical impact or playful reaction may need overshoot |
| An object leaves the frame | Accelerate into departure | A careful retreat or shrink may need a softer exit |
| An object changes position within the scene | Accelerate, then decelerate | Continuous transport may need constant speed |
| The camera follows an active object | Match the object's direction and speed | A deliberate reveal may need a separate camera move |
| A state changes immediately | A frame-aligned switch | A material transformation may need continuous motion |

These are starting choices, not measured benchmarks or universal rules.
Do not assign the same curve and duration to every element.
Use a small timing range appropriate to the brief, then inspect the result at delivery speed.

## Typography

Separate reading time from entrance and exit time.
The usable reading interval starts when the complete message is legible.
Use the final output size to judge type scale and line breaks.
Prefer phrase or word groups when the message needs rapid comprehension.
Use character-by-character animation when the act of typing is part of the product action.
Reserve large scale changes or a distinctive text effect for the word that carries the message.
Do not make every line the main event.

## Transitions

Choose the transition from the relation between shots.
Continue a gesture when the next shot shows its consequence.
Use a cut to change task, viewpoint, or context.
Use a dissolve when overlap or a gradual passage is meaningful.
Match position, scale, direction, or speed across a boundary only when continuity helps the viewer.
Do not force every shot into an object-transformation chain.

Check both sides of important boundaries, plus one intermediate state for continuous transitions.
Look for half-visible text, unintended overlaps, image exposure, and broken object continuity.

## Effects and depth

Choose an effect for a named purpose before adding it.
Use blur to show rapid travel or focus change; preserve enough time for a sharp result.
Use depth and camera movement to reveal shape, material, or a product relation.
Use generated footage or imagery as an asset when it supports the scene.
Keep precise brand text, actual product UI, and required geometry under composition control.
Do not treat 3D or a dark background as an automatic quality upgrade.

## Implementation and verification

Place every animation on the renderer's frame clock.
Compute layout constants after assets and fonts are ready, before timeline construction.
Avoid concurrent conflicting tweens on the same property of the same element.
Use nested layers when camera motion and local object motion need independent controls.
Prefer transforms for spatial animation unless the required shape change needs another method.
Verify the target state at the requested time and at the final frame.
For revisions, inspect the modified interval and its adjacent boundaries.
Report the edit, preserved properties, actual checks, and any unavoidable change.
