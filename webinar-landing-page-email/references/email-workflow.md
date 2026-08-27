# Webinar Email Workflow

Read this reference whenever the user requests one or more webinar emails.

## 1. Completeness gate

Do not draft or create an email file until all applicable information is confirmed.

### Common campaign information

- Webinar or episode identity
- Final or working public title, or confirmation that the new landing-page title will be used
- Event date, weekday, start time, and time zone or approved multi-time-zone display
- Speaker name and official title for every named speaker
- Latest approved landing page or, in Combined mode, the sources from which it will be created
- Requested email types
- Sender or sign-off convention when the organization requires one

### Type-specific requirements

**Newsletter / webinar invitation**

- Registration URL
- Primary audience or distribution context
- Confirmed event value proposition or approval to derive it from the landing page

**Registration confirmation**

- Confirmation subject convention, if one exists
- Calendar or attendance instructions
- Join-link policy: include a confirmed link, or explicitly confirm that it is delivered elsewhere or later

**One-day reminder**

- Final event time and time-zone display
- Confirmed join URL
- Approved support or contact instruction, if included

**Final reminder**

- Confirmed join URL
- Planned send timing, such as five or fifteen minutes before start

**Post-webinar follow-up**

- Recipient group: attendees, no-shows, or all registrants
- Recording URL
- Slides URL
- Final approved takeaways and any additional resource URLs
- Explicit confirmation of any unavailable resource that should be omitted

**Segmented sales invitation**

- Recipient segment and relevant current situation
- Personalization angle
- Sender identity and reply path
- Registration URL

### Gate behavior

If anything is absent or inconsistent:

1. List every missing or conflicting item in one numbered message.
2. Explain which selected email requires each item when it is not obvious.
3. Ask the user to supply or explicitly omit each item.
4. Stop. Do not draft text or create files.
5. Rerun the full gate after the reply.

An empty placeholder is not confirmation. A deliberate user instruction such as `omit slides from this version` is confirmation.

## 2. Shared content rules

- Use the latest landing page as the narrative bridge, then verify claims against authoritative sources.
- Keep each email focused on one lifecycle job.
- Do not copy the full `About the Webinar` or every learning bullet into an invitation.
- Keep title, preview, opening, bullets, and CTA from repeating the same promise.
- Preserve approved organizational formatting when a reference template is provided.
- Use exact, readable dates and time zones. Validate that the weekday matches the date.
- Keep public claims within the agenda and confirmed product evidence.
- Remove all residual details from reference emails before delivery.

## 3. Email-specific rules

### Newsletter / webinar invitation

Use this opening format unless the user supplies another approved convention:

```markdown
**Title:**
Webinar Invitation | [Webinar Title] | [Date and Time]

**Preview:**
[One concise reason to attend.]
```

Use two or three short body paragraphs:

> Recognizable audience problem → distinctive webinar value → speaker, format, or proof

Optionally include three to five scan-friendly takeaways. End with the confirmed registration CTA.

### Registration confirmation

Confirm successful registration, restate logistics, explain calendar or join-link delivery, and give one short expectation-setting summary. Do not resell the entire webinar.

### One-day reminder

Lead with `tomorrow`, restate the correct time and join action, and include only the most useful expectation or preparation note.

### Final reminder

Lead with the immediate start. Keep the body extremely short and make the confirmed join CTA dominant.

### Post-webinar follow-up

Thank the correct recipient group, present confirmed resources clearly, summarize only approved takeaways, and give a relevant next step. Do not claim a resource is attached or available unless its URL is confirmed.

### Segmented sales invitation

Write for the confirmed segment's situation and decision. Do not simulate personal knowledge that was not provided, and do not create fake personalization data.

## 4. Versioning and review

- Multiple selected types: `outputs/emails/[episode]-email-pack-v1.md`
- Single type: `outputs/emails/[episode]-[type]-email-v1.md`
- Create the next numbered version for substantive changes; never overwrite earlier versions by default.
- Before delivery, compare all dates, names, titles, links, and claims across the email set and latest landing page.
