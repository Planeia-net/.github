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
