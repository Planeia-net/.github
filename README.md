# Planeia-net organization standards

This repository is the canonical source for shared agent and writing standards used across Planeia-net repositories.

## Writing standards

Use [writing/index.md](./writing/index.md) as the router. Load only the files triggered by the task:

- Publishable prose -> [writing/human-writing.md](./writing/human-writing.md)
- Insurance content -> [writing/insurance-boundaries.md](./writing/insurance-boundaries.md)
- SEO / organic search -> [writing/seo-writing.md](./writing/seo-writing.md)
- Research, factual claims, statistics, legal/regulatory or current information -> [writing/source-policy.md](./writing/source-policy.md)

Project repositories should keep only brand-, product-, channel-, design-, and workflow-specific instructions locally. Shared standards should be linked here rather than duplicated.

## Repository bootstrap

For a new repository, copy the lightweight router from [templates/AGENTS.md](./templates/AGENTS.md). If GitHub Copilot repository instructions are used, also copy [templates/copilot-instructions.md](./templates/copilot-instructions.md) to `.github/copilot-instructions.md` in that repository.

GitHub organization-level Copilot custom instructions are configured in the organization settings, not inherited automatically from this repository.

## Shared Google Ads image skill

[Google Ads images](./.agents/skills/google-ads-images/SKILL.md) activates for requests such as "create google ads images" and reads [google-ads-images](./google-ads-images) for current sizes. Edit that reference file to change dimensions; the skill does not duplicate them.

## Shared image and video generation skill

[Image and video generation](./.agents/skills/image-video-generation/SKILL.md) covers realistic avatars, reference-derived angles, relighting, and continuity-aware motion. The root agent router and bootstrap templates link to this skill; they load it only for relevant requests, and it does not force photorealism.

The root agent router and bootstrap templates link to the Google Ads image skill. Existing repositories must load this router or add the same task-specific link to their instructions; updating templates does not update existing copies.

For a shared ChatGPT project, also add this rule when the project handles visual-generation requests, and ensure team members have connected GitHub access to this private repository:

> When someone asks to generate or edit images or videos involving realistic people or avatars, reference-derived camera angles, relighting, or continuity-aware motion, read and follow https://github.com/Planeia-net/.github/blob/main/.agents/skills/image-video-generation/SKILL.md. Load it only when relevant and preserve the requested visual medium and style.

For a shared ChatGPT project, add this rule to the project's instructions and ensure team members have connected GitHub access to this private repository:

> When someone asks to create Google Ads images, read and follow https://github.com/Planeia-net/.github/blob/main/.agents/skills/google-ads-images/SKILL.md and fetch https://github.com/Planeia-net/.github/blob/main/google-ads-images for the current size instructions before generating.

Saving a skill in GitHub does not install it in every ChatGPT conversation. Automatic use requires the host to load the skill or the project instructions above. No workspace-wide installation is implied by this repository change.
