---
name: image-video-generation
description: Create or direct images and videos involving realistic people or avatars, reference-derived camera angles, relighting, or continuity-aware motion. Trigger on image/video generation or editing requests when these techniques are relevant; do not impose photorealism when the brief calls for another style.
---

# Creating More Realistic Avatars

Use this guide when an image or video generation agent needs believable people, coherent shot variations, or deliberate lighting. Photographic realism is one possible creative direction, not a default for every brief. Follow the approved brief and reference material; do not promise that wording alone can guarantee realism, identity consistency, resolution, or artifact-free output.

## Principles for both image and video agents

1. **Honor the intended style.** Establish whether the brief calls for photography, illustration, animation, stylized CGI, or another medium. Use photorealistic direction only when it fits.
2. **Describe the scene in useful layers.** Specify the subject and action, environment, framing, light, materials, palette, mood, and important continuity details. Prefer concrete visual choices over piles of realism adjectives.
3. **Keep identity and continuity explicit.** Record the approved character or avatar's stable traits, wardrobe, accessories, and permitted likeness source. Identify which details may change from shot to shot. Possession of a reference photo does not establish consent to use a person's likeness.
4. **Treat camera terms as visual direction.** Lens, camera, aperture, and film references can suggest perspective and depth of field; they do not prove that a physical camera was used or guarantee a particular result.
5. **Use negatives selectively.** Add constraints such as “no plastic-looking skin” or “no unwanted text” only when relevant and supported by the selected generator. Do not assume every tool has a separate negative-prompt field.
6. **Inspect generated results.** Check identity, expression, anatomy, hands, reflections, object geometry, light direction, text, and continuity. Report defects plainly and request targeted revisions.

## Image generation: realistic people and avatars

Build a prompt from these elements, selecting only what the brief needs:

- **Person:** approximate adult age range when relevant, appearance, pose, expression, gaze, and action. Avoid unnecessary or unsupported identity details.
- **Framing:** close-up, medium, or wide shot; viewpoint; subject placement; background depth; and clear space for later graphics when needed.
- **Photographic character:** candid phone photo, documentary portrait, studio portrait, editorial image, or another specific photographic context.
- **Lighting:** plausible source and direction, softness, color temperature, shadow behavior, and bounce light. Examples include soft window light, overcast daylight, on-camera flash, and a motivated studio softbox.
- **Surface detail:** natural skin texture, hair strands, fabric weave, wear, or other details that are visible at the chosen framing. Include restrained imperfections when appropriate; do not make every person gritty or flawed by default.
- **Color and finish:** natural or intentionally stylized palette, contrast, grain, sharpness, and retouching level. Ask for subtle grain only when it serves the look.
- **Continuity anchors:** approved reference image, fixed wardrobe/accessories, environment layout, lighting direction, and any required visual traits.

Do not rely on “photorealistic,” “8K,” or a named camera to fix a vague prompt. Describe the visible result. Use tool-supported output settings for dimensions and upscaling, and distinguish requested quality from inspected quality.

### Example prompt

> Candid, photorealistic waist-up portrait of an adult woman speaking naturally to someone just off camera in a bright apartment living room. Eye-level framing, face in sharp focus, relaxed posture and conversational expression. Soft daylight comes from the window on camera left, with gentle shadow falloff and natural skin tones. Preserve visible skin texture, a few flyaway hairs, and the weave and folds of her simple cotton shirt. Cream sofa and textured cushions sit softly out of focus behind her. Neutral photographic color, restrained contrast. Keep her hairstyle, earrings, shirt, and the window-light direction consistent with the supplied character reference. No beauty-filter smoothing or added text.

Treat this as a starting point; replace details to match the actual brief. Do not reuse its subject, outfit, setting, or gender by default.

## Building multiple angles from a reference image

1. Choose a master frame with a clearly readable subject, lighting, and environment. Include foreground, middle distance, and background only when useful.
2. List the required coverage for the story: for example, establishing wide, medium action, close detail, over-the-shoulder, or reaction.
3. For each view, specify the camera position, framing, subject action, visible background, and what must stay fixed. Vary camera angle to clarify the scene, not just to produce more images.
4. Keep a continuity record for character traits, wardrobe, props, environment geometry, screen direction, and light source/direction.
5. Compare generated views with the master frame. Select and revise the usable angles; do not claim perfect identity or sequence accuracy without inspection.

If a supported product feature can derive views from a reference image (for example, Higgsfield SHOTS), use it only when the user has selected that tool or its availability is confirmed. Product names, interfaces, angle counts, and results can change; verify current capabilities instead of hard-coding guarantees.

## Relighting an existing image

When editing a generated or supplied image, first identify what should remain unchanged: subject identity, pose, framing, environment, and materials. Then specify the lighting change:

- source position or direction (side, top, back, or under);
- hard or soft quality;
- warmth/color and intensity;
- desired shadow, highlight, and mood changes; and
- any continuity target for other images in the same sequence.

Make a narrow lighting edit when the goal is lighting. Inspect the result for altered facial features, object shape, material color, reflections, and implausible shadows. If the selected tool cannot preserve these details, say so and offer a supported workflow. Relighting features such as Higgsfield Relight are optional and must be verified for current availability and supported inputs.

## Video generation: turn the visual direction into motion

Use a reference image or approved keyframe when available. For each shot, define:

- shot ID and duration requested by the brief;
- starting state and the subject's single primary action;
- natural secondary motion, such as blinking, breathing, hair, fabric, or background movement;
- framing and one purposeful camera movement, or a locked camera;
- lighting and environment behavior;
- identity, wardrobe, prop, screen-direction, and set details to preserve;
- final pose/state that can lead into the next shot; and
- audio direction only when the chosen setup supports it and the brief requests it.

Keep the motion physically plausible and readable. Break overloaded actions into separate shots. Avoid asking a still-image generator to create a moving sequence; use an image for the keyframe/reference and a video-capable tool for motion. Describe the opening and ending states so the result can be checked. Do not invent unsupported controls, durations, frame rates, camera paths, or sound features.

### Example motion prompt

> Starting from the supplied medium shot, the presenter looks toward the camera, gives a small natural smile, and raises the product to chest height over the requested shot duration. Keep the camera locked at eye level. Preserve the presenter's face, hairstyle, blue shirt, product shape, window position, and soft daylight from camera left. Allow subtle breathing and a small hand adjustment; keep the background still. End with the product steady and label facing camera for the next shot. Generate no extra text or speech.

## Handoff and review

For each requested asset, return the prompt or shot direction, required reference, continuity anchors, selected tool only when confirmed, and any unresolved limitations. After generation, review:

- subject identity, expression, anatomy, and hands;
- intended action, framing, and composition;
- lighting direction, shadows, reflections, and material appearance;
- continuity across angles or video frames;
- unwanted text, logos, watermarks, or graphic elements; and
- actual dimensions, duration, and audio only when relevant and measurable.

Distinguish planned checks from completed checks. A prompt that requests “natural,” “cinematic,” “8K,” or “no artifacts” is not evidence that the delivered asset meets those criteria.

## Related production instructions

- For character records, environment records, master frames, and image shot tables, see [image direction](images.md).
- For timed motion, voice, captions, and editing handoff, see [motion and editing](motion-editing.md).
