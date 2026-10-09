---
name: motion-review
description: "Review or repair a launch film or brand animation using the actual rendered video and available editable source. Use for motion QA, transition defects, readability, audio-picture coordination, or comparison of versions."
metadata:
  version: "0.1.0"
---

# Review launch motion

Base findings on the actual render and the brief.
Separate observed defects, measurable facts, and subjective preferences.
Do not certify a film's design quality from a successful render command.

## Inspect available evidence

Identify the requested result, actual video, source project, and previous approved version if relevant.
Use available media inspection tools to check duration, dimensions, frame rate, and planned audio.
Inspect representative frames and frames around important transitions.
A contact sheet is a grid of frames from different times in the video.
Use the installed renderer's snapshot tools or available media tools to produce one when useful.
Inspect playback when a playback tool is available.
If only stills are available, report that motion speed and audio remain unverified.
If source is absent, review the video and give timestamped repair guidance without claiming a source edit.

For a repair in fal Agent, use the existing `video-compositing` workflow.
In another agent, use the installed composition and rendering tools.
If repair tools are absent, provide findings and repair guidance without claiming an edit.
Preserve the user's approved scope and use the same source project where available.

## Review in consequence order

1. **Correctness:** Does the video decode and match the requested format and duration?
   Check missing assets, blank output, incomplete text, and unintended clipping.
2. **Product truth:** Does the scene show the actual product action or clearly identified illustrative content?
   Compare statistics, UI, copy, and claims with the supplied evidence.
3. **Comprehension:** Can the viewer identify the main subject and understand the visible result?
   Check text and product proof at delivery size, including usable reading time.
4. **Continuity:** Does each important transition preserve or deliberately change context?
   Inspect preceding, boundary, following, and intermediate frames where relevant.
5. **Motion:** Do speed, acceleration, overlap, and hold time serve the action?
   A static hold can be correct. An unintended blank interval is a defect.
6. **Finish:** Do type, color, imagery, materials, and effects form a consistent visual system?
   Treat a stylistic preference as a preference unless it conflicts with the brief.
7. **Audio:** If planned, does the mix support speech, reading, and important picture events?
   Inspect or measure audio with available tools. Do not claim an audible assessment from video stills.

A source lint or numerical threshold is evidence of a specific condition, not a verdict on taste.
Do not claim that every static frame is defective or impose a universal maximum end-card duration.

## Report and repair

For each material issue, record time, observed behavior, consequence, and the smallest useful repair.
Example: at 3.2 s, the second line is cut off; the benefit is unreadable; enlarge the text container.
Prioritize failures of the request and communication before cosmetic changes.
If asked only for a critique, deliver findings without editing the source.
If repair is authorized, fix the highest-impact issues first and re-render through the existing workflow.
Stop when the requested defects are resolved, or when a dependency prevents a reliable repair.
For broad polish, use a bounded pass and retain optional preferences for the user's choice.

## Compare variants

Use the same brief, assets, duration, and output format for a meaningful comparison.
State any uncontrolled difference in model, source, or production budget.
Prefer anonymous A/B presentation when the user wants to judge design quality.
Record the user's preference and reason only in the project's requested notes or available preference storage.
Do not assume this imported skill can modify its own installed files.

## Delivery note

State what was checked, what changed, what remained unchanged, and what remains uncertain.
Identify automated checks separately from visual or audible inspection.
Use a concise result such as: "The crop transition and final copy pass the checks described below. Audio remains unverified."
Keep review detail outside the film unless the user asks for an annotation or breakdown.
