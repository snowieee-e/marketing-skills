# Marketing Skills

Reusable personal marketing Skills managed through GitHub commit history and stable release tags.

## Webinar Landing Page

The executable Skill is stored in [`webinar-landing-page/`](webinar-landing-page/).

### How changes are recorded

- **Commits:** Each completed project produces one consolidated Skill update with a descriptive commit message. Open **History** on GitHub to see the files and exact lines added or removed.
- **Stable versions:** [`webinar-landing-page/VERSION`](webinar-landing-page/VERSION) uses semantic versioning. After a version change is pushed to `main`, GitHub Actions automatically creates a tag such as `webinar-landing-page-v1.0.0`.

Version rules:

- Patch: corrections without a workflow change, such as `1.0.0` → `1.0.1`.
- Minor: a new backward-compatible workflow or review capability, such as `1.0.0` → `1.1.0`.
- Major: a substantial incompatible redesign, such as `1.x.x` → `2.0.0`.

## Company-Aware Webinar Landing Page

The generalized Skill is stored in [`company-aware-webinar-landing-page/`](company-aware-webinar-landing-page/). It automatically builds a reusable company context from official company websites, product pages, documentation, or messaging materials before combining that context with webinar-specific sources.

Real company context stays in the user's project or approved private location and is never stored in the public reusable Skill. Its stable tags use the format `company-aware-webinar-landing-page-v1.0.0`.
