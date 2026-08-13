---
name: company-aware-webinar-landing-page
description: Create and revise technical webinar briefings and landing-page copy using both replaceable company context and evolving webinar sources. Use when Codex receives a company website, product pages, messaging or brand documents together with webinar outlines, presentations, whitepapers, videos, Feishu documents, or reviewer feedback, and must automatically build a reusable company context, generate a Chinese learning briefing and English Landing Page V1, or assess later company/webinar source revisions before creating new numbered versions.
---

# Company-Aware Webinar Landing Page

Create source-grounded webinar copy with a replaceable company layer. Keep the Skill generic: never write a real company's private context into this Skill directory.

## Workflow

### 1. Establish the project

Confirm or infer:

- Company and webinar/episode
- Available company sources and webinar sources
- Required public-copy sections and language
- Approximate word count
- Project folder and next landing-page version

Use this project structure when folders are appropriate:

```text
project/
├── company context/
│   └── company-context.md
├── data/
│   ├── source-index.md
│   └── briefings/
├── outputs/
└── work notes/
```

Keep real company context in the user's project or approved private location, never in the public Skill repository.

### 2. Build company context automatically

If a current `company-context.md` exists, read it before webinar sources. If it does not exist, ask the user only for available official company inputs, such as:

- Company homepage or About page
- Product or solution pages
- Official product documentation
- Messaging, positioning, or brand documents
- Approved customer or use-case pages

Do not ask the user to complete a long questionnaire. Read the supplied sources and create `company-context.md` using [company-context-template.md](assets/company-context-template.md).

Use this source priority:

1. Latest approved messaging, positioning, or brand guide
2. Latest official product documentation
3. Company and product web pages
4. Approved customer stories and use-case pages
5. Blogs and other supporting sources

For every context statement, distinguish:

- `明确表述`: directly supported by official company sources
- `归纳`: synthesized from multiple sources
- `需要确认`: incomplete, conflicting, permission-sensitive, or unsupported

Do not infer target audiences, differentiation, product relationships, claims, or brand voice more strongly than the sources allow. Ask one or two specific follow-up questions only when a missing answer would materially change the webinar copy.

### 3. Index both source layers

Create or update a source index that separates:

- Company sources: long-lived authority for naming, positioning, product relationships, audience language, claims, and voice
- Webinar sources: event-specific authority for agenda, speakers, topics, proof, demos, and episode boundaries

Company context answers `How should this company and its products be described?` Webinar sources answer `What will this session actually cover?`

When the two layers conflict, do not silently combine them. Flag the conflict and prefer the latest approved authoritative source for its domain.

### 4. Create the first briefing and landing page

For the first webinar source package, always create both:

1. A plain-language Chinese briefing under `data/briefings/`
2. English Landing Page V1 under `outputs/`

Do not require the user to approve the briefing first. The user can learn from and question the briefing while reviewing V1.

Use [pre-writing-briefing-template-zh.md](assets/pre-writing-briefing-template-zh.md). The briefing must show which understanding comes from company context, which comes from webinar sources, which is synthesized, and which requires confirmation.

Required sequence:

> Build/read company context → index webinar sources → create briefing → derive audience-led narrative → create Landing Page V1 → run claims and coverage audit

### 5. Analyze the decision audience

Identify primary and secondary personas using both source layers. Determine:

- Their current situation or architecture
- What they want to change
- Their strongest objection or uncertainty
- What decision the webinar helps them make
- What proof, demo, limitation, or practical answer would motivate registration

Do not assume all prospects share one setup. Add audience questions and `对 Landing Page 文案的启示` to the briefing.

### 6. Design the narrative

Use an audience-led decision path:

> Current situation or pain → company/product response → webinar learning path → proof or live experience → practical decision

Company context should improve accuracy and brand consistency, not turn the page into a generic company advertisement. Webinar sources still define the public promises.

For the initial package, create V1 immediately. For later material changes prompted by user feedback, discuss the logic chain before creating a new version.

### 7. Draft and audit the public copy

Create, unless the user requests otherwise:

- Title
- Subtitle
- `About the Webinar`, usually two short paragraphs
- Four to six distinct `What You'll Learn` bullets
- Optional audience section, CTA, or short description

Read [copy-and-review-rules.md](references/copy-and-review-rules.md) before public drafting or revision. Use [landing-page-template.md](assets/landing-page-template.md).

Audit every public promise against both source layers:

- Webinar agenda supports the promised content
- Company/product naming follows official context
- Claims are confirmed, attributed, or flagged
- Competitive comparisons are fair and dimension-specific
- Customer names, metrics, and roadmap items have permission and evidence
- Important webinar content is not missing
- Other episodes are not mixed into the current page

### 8. Handle later source revisions

When the user supplies a newer company or webinar source:

1. Compare it with the current source index, company context, briefing, and latest landing page.
2. Before editing files, explain in the conversation:
   - What understanding changed, was added, or was removed
   - Whether it affects company context, the briefing, the landing page, or all three
3. Wait for the user's confirmation.
4. After confirmation, add a new numbered, dated update note at the top of the affected context or briefing file. Keep the original body; do not silently rewrite history.
5. Create the next numbered landing-page version if public copy is affected. Never overwrite an earlier version.
6. Update the source index and project update log.

Use newest-first update notes containing source/revision, changed understanding, affected sections, and landing-page impact.

### 9. Preserve revision reasoning

Place a concise internal `Logic Chain` above each numbered landing-page draft and outside public copy.

Maintain a separate project update log. For every version record:

- `Problem`
- `Why It Matters`
- `Change`
- `Learning`

Keep version-to-version notes out of the landing-page body.

### 10. Close the project and improve the Skill

During active copy development, update project notes rather than the Skill.

When the user gives a project-close instruction:

1. Review the complete update log and retrospective.
2. Separate company- or project-specific observations from reusable rules.
3. Update the user's playbook.
4. Make one consolidated Skill update only when the method genuinely improved.
5. Scan for company-specific or sensitive content before any public GitHub commit.
6. Validate the Skill and use descriptive Git commit history and stable semantic-version tags.

Never add a real company's `company-context.md` to this reusable Skill.
