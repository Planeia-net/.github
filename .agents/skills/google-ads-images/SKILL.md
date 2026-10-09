---
name: google-ads-images
description: Create or adapt Google Ads images using the shared Planeia-net size instructions. Trigger on "create google ads images", Google Ads image ads, Performance Max/PMax images, or equivalent requests such as "criar imagens para Google Ads".
---

# Google Ads images

## Load the size instructions first

Read the current canonical file before planning or generating images:
https://github.com/Planeia-net/.github/blob/main/google-ads-images

With the GitHub connector, fetch repository `Planeia-net/.github`, path `google-ads-images`, using its default branch. In an up-to-date checkout of that repository, read the root file `google-ads-images`.

This file is the source of truth for recommended pixel dimensions, minimum dimensions, aspect ratios, and maximum file size. Do not duplicate its numeric specifications in this skill, substitute remembered sizes, or silently use a different standard. If it cannot be read, ask for access or the file contents before generating size-dependent deliverables.

## Apply to the request

For photorealistic people or avatars, reference-derived angle variations, relighting, or continuity-aware motion in the brief, also follow the shared [image and video generation skill](https://github.com/Planeia-net/.github/blob/main/.agents/skills/image-video-generation/SKILL.md). It supplements this skill and does not replace its size and export requirements.

1. Use the current conversation and applicable repository brand instructions for the brief. Ask only for missing information needed to produce the requested images, such as brand, product, language, message, or concept count. Do not infer Planeia versus Seguro de Portugal from this shared skill.
2. Use the recommended dimensions in the canonical file for the requested formats. For a complete set without a narrower format request, include every format listed there. For a named campaign or placement with uncertain supported formats, clarify or verify the placement before promising upload compatibility; the shared file is a size reference, not a complete placement policy.
3. If the user explicitly requests a different size, identify the departure from the reference and follow their instruction. Never describe an out-of-spec export as compliant with the reference.
4. Create each concept/format as an individual image. Adapt composition to the target aspect ratio; keep text, logos, and focal subjects clear of crop edges. Do not stretch the artwork or deliver a contact sheet as the individual ad assets.
5. Use an available image-generation/editing tool according to its instructions. If it cannot export the exact required dimensions or file size, state that limitation and identify any remaining export step. Do not claim exact sizing merely because the prompt requested it.

## Verify and deliver

- Inspect actual exported width, height, and file size when accessible, and compare against the canonical file.
- Use recommended pixel dimensions as the primary export target; retain the file's published dimensions even when a displayed ratio is rounded.
- Check legibility and cropping for each format. A minimum-size pass does not mean the recommended size was achieved.
- Label each delivered asset by concept and format, and report actual dimensions and file size when verified. Clearly label any checks that could not be performed.
- Follow the host's delivery and saving rules. Do not claim Google approval or upload readiness based on dimensions alone.
