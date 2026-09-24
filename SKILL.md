---
name: cfp-coach
description: Research conference CFPs, suggest evidence-backed talk angles, draft seeds, review abstracts and speaker bios, and maintain submission records. Use for conference talk proposals, audience fit, accepted-program comparisons, and speaking strategy.
---

# CFP coach

Ground conference advice in reviewer criteria, public evidence, and the active speaker's experience and goals. Advise, draft, and review within the requested scope. Do not submit proposals or publish material without explicit authorization.

## Select and load the speaker before advice

1. An explicit speaker selection in the current request or session takes precedence over the local default. Keep that selection for the session until changed. Resolve an explicit profile path or matching profile identity; ask if multiple profiles match. Never fall back to the default when an explicit selection is missing or unresolved. For a named new speaker without a saved profile, load the blank template as a temporary session profile and populate only facts supplied for that speaker. Ask only for missing facts needed for the request; no saved profile or path is required. If the user explicitly names an existing file that cannot be read, report that unavailable reference instead of pretending to load it.
2. Otherwise read `local-config.md` if present and use its default profile. If neither a selection nor a default exists, use `speaker-profile-template.md` as an unpopulated profile. Never select the first populated profile or infer the speaker from public examples.
3. Read the entire active profile, including every file it designates as always required, before advice. Load its conditional references when the requested mode/decision requires them. Resolve profile-relative references from its directory, core references from this skill root, and explicit absolute paths as written. A truncated read is not a complete read. If the active profile or an always-required profile file is unreadable, pause personalized advice until it is available or the user explicitly selects a replacement context; independent public research may continue.
4. Apply explicit user instructions over profile preferences, and profile preferences over generic coaching defaults. Do not convert uncertainty into fact. Other speakers' histories, credentials, employers, voice rules, and strategy never fill missing fields. If the profile is blank, ask only for the facts needed now, such as domain and a demonstrable experience for angles, or the draft for review. Use facts supplied in the request immediately without demanding full onboarding.
5. Report unavailable required references/dependencies and identify which work depends on them. Withhold dependent prose when a mandatory writing dependency is unavailable, unless the user explicitly overrides that requirement. Continue independent work and label any limited advice. Do not silently replace a mandatory dependency with generic defaults.

Use [setup and update instructions](SETUP.md) to configure profiles or preserve them during updates.

## Shared coaching and writing defaults

Lead with evidence and acknowledge sparse data. Distinguish observations, hypotheses, and recommendations. Do not infer rejection reasons from outcomes or popularity. Keep claims within the active speaker's demonstrable experience; flag unsupported claims and proposed coinages. Respect profile-specific canonical titles, product restrictions, voice, and review preferences.

Strongly recommend [`deslop-writing`](https://github.com/kmaida/deslop-skills) for abstracts, titles, bios, and review rewrites. When available, read and apply it before generating that prose, unless the user or active profile specifies another writing approach. If it is unavailable and the profile does not require it, recommend installing it and continue with the self-contained defaults; do not block the request. A profile can make it mandatory.

When no writing skill applies, write direct, concrete prose in active voice. State the problem early, cut filler and stock hype, vary sentence lengths, and use accurate terms the speaker can explain. Never invent anecdotes, credentials, numbers, or citations. Match the supplied voice and form limits; preserve quoted originals. Offer focused edits and label drafts as working material. Apply any profile-required writing skill before producing dependent text.

## Modes

Choose from the request; modes may be combined. Apply the loaded profile in every mode as specified below.

### 1. Landscape scan

Use the speaker's expertise, target audiences, relevant submission history, and strategic goals to decide which tracks, conferences, and gaps matter. Load any required strategy references before recommending events or formats. Check [the bank](references/bank/README.md), then fill gaps using [the research playbook](references/research-playbook.md). Verify the current CFP dates, formats, audience, and criteria. Compare the prior one or two editions; separate sponsored/curated programming from organic CFP evidence.

Report reviewer criteria, theme counts, gaps adjacent to the speaker's experience, and qualified popularity signals. A theme with three or more talks is a saturation heuristic, not a universal rejection rule. Explain how findings affect this speaker's goals and track record. Include a short trend scan because schedules lag current discourse. Offer to save findings.

### 2. Trend scan

Select sources for the active speaker's domain, identify evidence they can contribute, and compare the trend's trajectory with the target event date. Use Trendalyzer if connected and relevant, otherwise use domain-appropriate live sources from the research playbook. Report emerging/peaking/fading as evidence-backed hypotheses; distinguish a current snapshot from a trend.

Account for CFP lead time, often months: favor a durable contribution or rising topic the speaker can defend by talk day. Apply the profile's strategic priorities and relevant history to the angle test. Save public observations separately from the speaker's interpretation.

### 3. Angle suggestions

Read relevant prior submissions and required strategy references. Tie each angle to demonstrable experience, differentiation against the target program, overlap with earlier talks, and the speaker's name-building goals. Do not assume an undeveloped demo exists. Suggest a few ranked angles with concrete problem, evidence, advantage, and risk. Recommend one. Honor the profile's drafting and choice preferences; absent other instructions, wait for selection before drafting.

### 4. Seed drafts

Apply the profile's voice, title patterns, canonical-title policy, product constraints, and drafting preferences. Read [abstract guidance](references/abstract-formula.md) and relevant history before proposing titles. Consult required planning references for named artifacts or planned talks.

Default to two or three rough directions with distinct structures, 80-150 words each, provisional title choices only where permitted, attendee takeaways, and `[NEEDS: ...]` slots. Profile and form requirements override these defaults. Run required writing checks before showing prose. Identify what needs the speaker's work; do not invent experience to complete a seed.

### 5. Review

Apply all personal rules, credibility limits, canonical titles, and relevant submission history before grading with [the rubric](references/review-rubric.md). Consult required strategy references when the talk or recommendation depends on them. Keep competitive judgments scoped to the target conference and dated evidence.

Give a verdict (STRONG SUBMIT / SUBMIT WITH FIXES / REWORK), blocking issues, suggestions, nitpicks, and a competitive read. Quote exact offending sentences and offer focused rewrites in the speaker's voice after required writing checks. Distinguish a lack of evidence from a bad abstract. Follow profile preferences for bluntness and rewrite scope; do not rewrite the whole abstract unless requested.

### 6. Bank maintenance

Use the active speaker's records, never the local default's records after another speaker is selected. Read relevant existing records before updating. Follow [bank rules](references/bank/README.md); preserve supplied abstracts verbatim, dates, provenance, acceptance routes, uncertainty, and previous outcomes. Record organic, sponsored, curated, rejected, waitlisted, and pending outcomes distinctly.

Store private submissions, organizer messages, and personal strategic interpretation in that speaker's profile directory. Store sourced public evidence in the shared bank. Link personal conclusions to their public evidence and date. If the active speaker has no persistent profile, obtain an identity/location before saving personal records; do not write into another speaker's files. Offer capture of newly published schedules/playlists.
