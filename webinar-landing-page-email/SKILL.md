---
name: webinar-landing-page-email
description: Create, revise, and audit source-grounded technical webinar briefings, landing pages, and coordinated email campaigns. Use when Codex must produce a Chinese pre-writing briefing, concise English landing-page copy, webinar invitation or lifecycle emails, or a combined landing-page-and-email package from outlines, decks, whitepapers, videos, messaging, live documents, and reviewer feedback.
---

# Webinar Landing Page and Email

Turn technical webinar sources into a coherent campaign: a learning-oriented Chinese briefing, an audience-led English landing page, and requested webinar emails. Keep internal reasoning separate from public copy and never promise more than the approved sources support.

## Choose the deliverable mode

Infer or confirm one of three modes:

1. `Landing Page`: briefing plus Landing Page V1, or a new landing-page revision.
2. `Email`: requested emails based on the latest approved landing page and event details.
3. `Combined`: briefing, landing page, and requested email set as one campaign.

Do not generate emails merely because the task concerns a webinar. Email is included only when the user requests it.

## Establish the project

Confirm or infer:

- Webinar or episode and requested deliverables
- Required language, sections, length, and output format
- Latest source package and current approved copy
- Project folder and next version number
- Requested email types, if any

Adapt to an existing project structure. For a new project, use:

```text
project/
├── data/
│   ├── source-index.md
│   └── briefings/
├── outputs/
│   ├── landing-pages/
│   └── emails/
└── work notes/
```

Never overwrite numbered drafts unless the user explicitly requests it.

## Build the source hierarchy

Use this priority:

1. Latest approved agenda, deck, or speaker outline: authority for what the session covers.
2. Official messaging and product documentation: authority for naming, positioning, and product claims.
3. Whitepapers and technical references: authority for explanations and supporting facts.
4. Approved customer evidence: authority for proof points and metrics.
5. Latest approved landing page: authority for the campaign narrative, but not a substitute for source verification.
6. Existing emails and reviewer comments: format and direction, not automatic factual authority.

Record conflicts and unresolved claims. Recheck the revision or modified date of live sources before final delivery.

## Enforce the email information gate

Whenever the requested deliverables include email, read [email-workflow.md](references/email-workflow.md) and run its completeness gate before drafting or creating any output file.

- Check the common event fields and the fields required by every selected email type.
- Treat conflicting dates, weekdays, time zones, speaker details, links, or titles as missing information.
- Ask for all missing or conflicting items in one consolidated message.
- Stop and wait for the user's reply. Do not create a partial email, placeholder-filled draft, or email file.
- After the reply, rerun the gate. Draft only when every required item is confirmed or the user explicitly marks an item as intentionally omitted or not applicable.

In `Combined` mode, complete this gate before creating the combined public-copy package. Landing-page-only requests do not require email logistics.

## Create the pre-writing briefing

For the first source package, create a plain-language Chinese briefing under `data/briefings/` using [pre-writing-briefing-template-zh.md](assets/pre-writing-briefing-template-zh.md).

The briefing must include:

- Source information and the source's original outline
- `转述`, `归纳`, and `需要确认`
- A one-sentence summary and reorganized briefing outline
- Primary and secondary personas, their current situation, and their questions
- Central claim, mechanism, proof, practical takeaway, limitations, and risky claims
- Implications for both landing-page and email copy when email is in scope

Do not copy the briefing into public copy. Use it to prevent vague or technically confused marketing language.

## Design the campaign narrative

Use one shared decision path:

> Audience situation → why it matters now → webinar approach → distinct learning outcomes → proof or live experience → action

The landing page explains the full registration case. The invitation email selects the strongest angle and drives the reader to the page; it must not duplicate the entire landing page. Confirmation, reminder, and follow-up emails serve their lifecycle purpose instead of retelling the whole narrative.

If the source covers a series, map episode boundaries before drafting and keep each claim, example, and CTA with the correct episode.

## Draft the landing page

Unless the user requests another format, create:

- Title and audience-led subtitle
- `About the Webinar`, usually two short paragraphs
- Four to six distinct `What You'll Learn` bullets
- CTA placeholder or confirmed CTA
- Optional audience section or short description

Read [copy-and-review-rules.md](references/copy-and-review-rules.md) before drafting or revising. Use [landing-page-template.md](assets/landing-page-template.md).

For the initial package, create the briefing and Landing Page V1 together after any applicable email gate is complete. Do not require separate approval of the briefing first.

## Draft the email set

Generate only the email types selected by the user. Supported types are:

- Newsletter or webinar invitation
- Registration confirmation
- One-day reminder
- Final reminder
- Post-webinar follow-up
- Segmented sales invitation, only when the audience segment and personalization angle are confirmed

Use [email-pack-template.md](assets/email-pack-template.md) and follow [email-workflow.md](references/email-workflow.md).

Default to one versioned email-pack file when multiple types are requested, for example `episode-01-email-pack-v1.md`. When only one email is requested, use a type-specific versioned filename. Keep internal confirmation notes above the public-copy divider and out of the send-ready text.

## Audit the campaign

Verify both landing page and emails against the newest sources:

- Every public promise belongs to the approved agenda.
- Product names, relationships, and versions follow official messaging.
- Customer evidence, metrics, comparisons, and roadmap statements have exact support and permission.
- Dates, weekdays, times, time zones, speakers, and URLs agree across every asset.
- CTA destinations match the lifecycle stage.
- No text, title, speaker, date, link, or product detail remains from another webinar or email template.
- Invitation copy adds a focused reason to click instead of repeating the landing page.
- Confirmation and reminder copy stays operationally clear.
- Follow-up resources and takeaways are final and available.

Report unresolved issues instead of polishing around them.

## Handle revisions

When new sources or reviewer feedback arrive:

1. Compare them with the source index, briefing, latest landing page, and latest email set.
2. Explain what changed and which campaign assets are affected before editing.
3. Wait for confirmation when the change materially affects the narrative or comes from a revised source.
4. Add a newest-first update note to the briefing when source understanding changes; do not rewrite its original body silently.
5. Create new numbered versions only for affected public assets.
6. Update the source index and project update log.

For each public-copy version, record `Problem`, `Why It Matters`, `Change`, and `Learning` in the project update log. Keep company-specific context, private links, customer information, and unpublished claims out of this reusable Skill.
