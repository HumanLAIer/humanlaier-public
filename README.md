# PRODUCTION OUTPUT ONLY — DO NOT EDIT HERE

> [!CAUTION]
> **This is the public deployment repository for [humanlaier.com](https://humanlaier.com/). It is not the website's editing or source repository.**
>
> **Do not edit files here using Pages CMS, GitHub's web editor, GitHub Desktop, or direct pushes.**
> Manual edits can be overwritten during the next approved release, introduce changes that bypass source review, or interrupt production.

## Where to make changes

**Use the private source repository: [HumanLAIer/humanlaier-website](https://github.com/HumanLAIer/humanlaier-website).**

- **Copy and visual experiments:** Open [Pages CMS](https://app.pagescms.org), select `humanlaier-website`, and explicitly choose the `editorial` branch.
- **Technical changes:** Work in a dedicated branch of `humanlaier-website` and propose a pull request.
- **Release approval:** Review and merge approved changes to `humanlaier-website`'s `main` branch.
- **Publishing:** The [approved-domain GitHub Actions workflow](https://github.com/HumanLAIer/humanlaier-website/blob/main/.github/workflows/publish-approved-domain.yml) builds the approved source and deploys the resulting static files to this public repository.

Only approved publishing automation and authorized release administrators should write to this repository.

## Repository and website map

| GitHub repository shown in Pages CMS | What it is | Web address | Edit in Pages CMS? |
| --- | --- | --- | --- |
| [`humanlaier-website`](https://github.com/HumanLAIer/humanlaier-website) (private) | Website source; `main` = approved, `editorial` = creative drafts | Source repository, **not** a directly hosted URL; its approved `main` publishes to [humanlaier.com](https://humanlaier.com/) | **YES — only the `editorial` branch** |
| [`humanlaier-public`](https://github.com/HumanLAIer/humanlaier-public) (public) | Compiled production deployment output | **[humanlaier.com](https://humanlaier.com/)** | **NO — DEPLOYMENT ONLY** |
| [`humanlaier.github.io`](https://github.com/HumanLAIer/humanlaier.github.io) (public) | Separate legacy/prototype hosting and editorial preview | [humanlaier.github.io](https://humanlaier.github.io/) and [humanlaier.github.io/editorial/](https://humanlaier.github.io/editorial/) | **NO — preview publishing output** |
| [`hl-livestream-pilot`](https://github.com/HumanLAIer/hl-livestream-pilot) (private) | Separate livestream research/prototype | No company website domain established by this deployment | **NO — not the corporate website** |

The URLs above are **hosting destinations**, not alternate Pages CMS editing endpoints. Pages CMS works on the selected GitHub repository and branch.

## Production publishing precautions

- This repository must remain **public** to host the website under the current GitHub Pages setup.
- The `CNAME` file contains `humanlaier.com`; **do not change or delete it**.
- The approved publisher preserves `README.md`, `CNAME`, and `.nojekyll` when synchronizing generated files.
- **Do not archive the repository, make it private, or lock its `main` branch** without first verifying that the approved publishing credential can still push deployments.
- The human-review and least-privilege access controls should be configured in GitHub organization/repository settings, without disabling the automated publisher.

**Site maintenance and editorial handoff:** [docs/EDITORIAL-STUDIO-STATUS.md](https://github.com/HumanLAIer/humanlaier-website/blob/main/docs/EDITORIAL-STUDIO-STATUS.md) in the private source repository.
