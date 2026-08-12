---
name: webinar-landing-page
description: Create, revise, and audit concise English landing-page copy and Chinese pre-writing briefings for technical webinars from outlines, whitepapers, messaging guides, presentations, videos, Feishu documents, and reviewer comments. Use when Codex receives the first source package for a webinar and must generate both a learning-oriented briefing and Landing Page V1, or when later source revisions require an impact analysis, append-only briefing update, and new numbered landing-page version.
---

# Webinar Landing Page

Turn technical source material into concise, audience-led webinar copy. Separate internal reasoning from public copy, and never let the landing page promise more than the speakers will cover.

## Workflow

### 1. Establish the deliverable

Confirm or infer:

- Webinar episode and topic
- Required sections and language
- Approximate word count
- Whether audience information belongs in the public copy
- Output folder and next version number

If the project already uses numbered Markdown versions, create the next version and never overwrite an earlier file unless the user explicitly asks.

### 2. Build a source hierarchy

Read the latest available materials and classify them:

1. Latest approved agenda, deck, or speaker outline: authority for what the webinar covers.
2. Official messaging or product documentation: authority for naming, positioning, and product claims.
3. Whitepapers and technical references: authority for explanations and supporting facts.
4. Customer evidence: authority for proof points, subject to approval and exact sourcing.
5. Existing copy and reviewer comments: evidence of direction, not automatic factual authority.

Record unresolved conflicts instead of silently choosing a convenient claim. Recheck the revision or modified date of live documents before final delivery.

### 3. Create a pre-writing briefing and first draft

When the user provides the first source package for a new webinar, always create a plain-language Chinese briefing. This is mandatory regardless of whether the package contains one simple document or multiple complex sources. Save it under `data/briefings/` when the project uses folders; create that folder if needed.

Generate Landing Page V1 in the same initial delivery after completing and auditing the briefing. Do not require the user to approve the briefing first. The briefing is the learning layer the user can read and question while reviewing the first draft.

Use this order:

1. Source information: title, link/path, revision/date, and purpose of the briefing.
2. Original source outline: preserve the source's own logic and section order.
3. Content-basis note with three groups:
   - `转述`: facts and plain-language paraphrases directly grounded in the source.
   - `归纳`: audience, narrative, or positioning conclusions synthesized from multiple source sections.
   - `需要确认`: permissions, metrics, speaker details, agenda status, and live-document revisions.
4. One-sentence summary.
5. Briefing outline: reorganize the explanation for the reader; keep it distinct from the original source outline.
6. Briefing body.

The briefing body should explain:

- What changed or why the topic matters now
- The audience's current setup and pain
- The questions each audience segment wants the webinar to answer
- The webinar's central claim
- The mechanism or product story supporting that claim
- The proof, demo, or practical takeaway
- Important limitations, fair counterpoints, and risky claims

Use clear heading groups rather than a flat list of unrelated sections. Keep the original source outline and the briefing outline synchronized with their respective content.

Do not copy the briefing into the landing page. Use it to prevent vague or technically confused marketing language.

For the initial source package, the required output sequence is:

> Read sources → create/update source index → create briefing → derive narrative → create Landing Page V1 → run claims and coverage audit

### 3A. Handle later source revisions

When the user provides a newer outline, deck, document, video, or other source after drafting has begun:

1. Read and compare the new source with the source index, current briefing, and latest landing-page version.
2. Before editing files, explain in the conversation:
   - Which prior understandings have changed, been added, or been removed.
   - Whether and how those changes affect the current landing page.
3. Wait for the user's confirmation before updating either the briefing or landing-page copy.
4. After confirmation, preserve the existing briefing body and add a new numbered, dated update note at the top of the same briefing file. Do not silently rewrite or replace the earlier briefing analysis.
5. The top update note must identify the new source/revision, changed understanding, affected briefing sections, and impact on the landing page.
6. Create the next numbered landing-page version; never overwrite the current version.
7. Update the source index and version update log so the latest source and resulting copy change remain traceable.

Use this update-note pattern, with the newest entry first:

> `Briefing Update 2 — [date / source revision]` → Changed understanding → Affected sections → Landing-page impact

### 4. Audit series and episode boundaries

If the source covers multiple sessions or episodes, build a boundary map before drafting:

- What belongs to each episode
- What is shared series context only
- Which audience belongs primarily to which episode
- Which customer evidence supports which episode and claim
- Which topics must not cross into the current episode

Verify both episode sections against the latest source instead of relying on a prior summary. Label shared market narrative or evidence clearly so it is not mistaken for current-episode agenda content.

### 5. Identify the decision audience

Determine:

- Primary persona and secondary personas
- What they already know
- What they operate today
- What they want to change
- Their strongest objection
- What decision the webinar helps them make

For each primary and meaningful secondary persona, derive a short question set from the source:

- What capability difference do they need explained?
- What operational or architectural concern do they need evaluated?
- What proof would make the session credible to them?
- What limitation or counterpoint do they expect the speaker to acknowledge?
- What practical demo or AMA question would motivate registration?

Add these questions to the briefing after each persona, then add a short `Implications for Landing Page Copy` section. Use it to decide the opening problem and learning points. Do not force every question into public copy, and do not introduce questions that belong to another episode.

Write the page for the primary persona without implying that all registrants have the same background. If no `Who Should Attend` section is requested, express the audience through the opening problem and learning outcomes.

### 6. Discuss and design the narrative

Organize the public copy as a decision path, not a feature inventory:

> Current problem → why it matters now → webinar approach → distinct learning outcomes → proof or live experience → CTA

The second paragraph of `About the Webinar` must answer the problem raised in the first paragraph. Its final sentence should summarize the webinar at a high level rather than repeat every bullet.

For the initial source package, create the briefing and Landing Page V1 together without an approval gate. For later copy revisions prompted by user feedback, discuss the proposed audience, core tension, narrative sequence, learning-point scope, exclusions, and unresolved questions before creating a new version when the change is material. For later source revisions, always follow the confirmation gate in Step 3A.

### 7. Draft the copy

Unless the user specifies another format, create:

- Title
- Subtitle
- `About the Webinar`: usually two short paragraphs
- `What You'll Learn`: usually four to six bullets
- CTA placeholder
- Optional short description when requested

Use the Markdown structure in [landing-page-template.md](assets/landing-page-template.md). Read [copy-and-review-rules.md](references/copy-and-review-rules.md) before drafting or revising public copy.

### 8. Run a claim and coverage audit

For every public promise, verify:

- The latest agenda or deck actually includes it.
- Product names and relationships follow official messaging.
- Comparisons use consistent dimensions and remain fair.
- Customer numbers and technical claims have a source.
- Roadmap items are not presented as available features.
- The language does not convert “supports” into “guarantees.”
- Paraphrases and synthesized conclusions are not presented as direct source statements.
- Customer naming permission and published metrics are confirmed before public use.

Compare the draft against the newest source material in both directions:

- Important source topic missing from the copy
- Copy promise absent from the source

### 9. Polish for scanning and flow

Check that:

- Each bullet answers one different audience question.
- Bold bullet headings use one parallel form; prefer concise noun phrases.
- Explanations start with a clear action verb and state a concrete takeaway.
- Architecture, security, deployment, proof, and operations do not repeat one another.
- Technical component lists appear only when they help the decision.
- The opening, bullets, and short description do not repeat the same wording.
- The public body meets the requested word count.

### 10. Deliver with useful internal context

When useful, place a short internal note above a divider containing:

- A concise logic chain showing how the public narrative progresses
- Target audience
- Narrative logic
- Items requiring speaker, product, legal, or messaging confirmation

Keep these notes clearly outside the public landing-page copy.

When a project uses numbered landing-page versions, keep version-to-version changes in one separate update log rather than repeating them at the top of each draft. For every version, add a numbered entry with:

- `Problem`: the specific issue or feedback that prompted the version.
- `Why It Matters`: why the issue affects audience relevance, clarity, credibility, or conversion.
- `Change`: the corresponding content, positioning, or structural revisions.
- `Learning`: the potentially reusable writing insight revealed by the revision.

Preserve the earlier entries and keep the log synchronized whenever a new copy version is created.

For projects that use this review format, place a one-line `Logic Chain` above every new numbered draft and before the public-copy divider. Keep it concise and directional, for example:

> Audience requirement → product capability → proof or comparison → practical takeaway

The logic chain is an internal review aid and must not appear in the published landing page.

## Revision Behavior

- Discuss narrative logic before a major rewrite when the user requests discussion.
- When feedback targets one sentence, check whether it reveals a larger audience or positioning issue.
- Preserve user edits and existing versions.
- Use precise, plain language; do not resolve uncertainty with polished but unsupported wording.
- Update the project work log after a confirmed strategic change when a log exists.
- During active copy development, record candidate learnings in the project update log and personal playbook; do not repeatedly modify the Skill for each draft-level change.
- Treat a user statement such as `本次 webinar landing page 文案写完了，帮我总结并将可复用的经验沉淀到 skill` as the project-close trigger. At that point, review the complete update log, separate project-specific observations from reusable methods, complete the project Skill retrospective, update the personal playbook, and then make one consolidated Skill/template update.
- Keep project work notes focused on three purposes: version-update evidence, end-of-project Skill retrospective, and the user's personal copywriting playbook. Do not create multiple project-local workflow-version files when the executable workflow already lives in the Skill.

## Skill Release and GitHub Versioning

During an active webinar project, record draft-level learnings in the project update log; do not create a Skill commit for every copy revision.

When the user gives the project-close trigger and asks to sync the Skill to GitHub:

1. Complete the retrospective and separate project-specific details from reusable rules.
2. Make one consolidated update to the Skill, references, and templates.
3. Scan the complete Skill directory for company-specific material, customer information, internal links or paths, credentials, personal data, and unpublished claims. Stop and report any risky content before committing.
4. Validate the Skill structure and frontmatter.
5. Review the Git diff and write one descriptive imperative commit message that states the reusable improvement, such as `Improve revised-source briefing workflow`.
6. Update the adjacent `VERSION` file only when publishing a stable release:
   - Patch, for corrections that do not change the workflow: `1.0.0` → `1.0.1`.
   - Minor, for a new backward-compatible workflow or review capability: `1.0.0` → `1.1.0`.
   - Major, for a substantial incompatible redesign: `1.x.x` → `2.0.0`.
7. Commit the consolidated change and push it to the configured personal GitHub repository when the user has authorized project-close synchronization. If push authentication is unavailable, leave the verified commit ready and ask the user to click `Push origin` in GitHub Desktop.
8. Let the repository workflow create the stable tag from `VERSION`. Do not manually maintain duplicate `SKILL-v1`, `SKILL-v2`, or changelog copies.

Use commit history to explain every concrete change and stable tags to identify release milestones.
