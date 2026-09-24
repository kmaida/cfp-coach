# Research playbook

How to gather acceptance and popularity evidence when the bank has gaps. Bank first, always; this playbook fills what's missing.

## 1. Current CFP guide

Search for `<conference> <year> CFP` or check Sessionize/PaperCall directly (most AI and dev conferences use Sessionize: `sessionize.com/<conference-slug>`). Capture:

- Submission deadline, notification date, event dates
- Session formats and lengths
- Track list and stated audience
- Explicit review criteria (many CFPs publish "what we look for"; this is gold, quote it tightly)
- Form constraints: character limits, required fields, video asks

## 2. Prior schedules

Search `<conference> <prior year> schedule` or `agenda`. Sources in order of reliability: the conference site's archived agenda, Sessionize public schedule pages, press coverage roundups. For each relevant track, capture accepted titles and abstracts. Two prior years beats one; three is diminishing returns.

If the conference is new (no prior editions), use analogs: same organizer's other events, or conferences with the same audience. Say explicitly that the data is analog-based.

## 3. YouTube popularity signals

Search `<conference> <year> playlist site:youtube.com` or the organizer's channel. Capture per-video: title, speaker, view count, publish date.

Normalize before comparing:

- Views decay-adjust: older videos accumulate more views. Compare within the same edition, not across years.
- Keynote and celebrity bias: strip keynotes and famous-name speakers before reading topic signal.
- Title bias: provocative titles draw clicks independent of topic. Note when a view spike is probably the title, because that itself is a useful title lesson.

What the signal is good for: which topics the audience seeks out after the event. What it's not: a proxy for what the committee accepts. Keep the two separate in reports.

## 4. Acceptance-side signals

- Speakers who appear across multiple editions: the committee trusts them; their topics show committee taste.
- Track composition shifts year over year: a track that grew is a demand signal, one that shrank is saturation or pivot.
- Public acceptance-rate statements or committee blog posts ("we received 800 submissions for 90 slots") calibrate how sharp the differentiation needs to be.

## 5. Saturation math

For the target track and the last two editions, cluster accepted talks by theme. A theme with 3+ talks is saturated: submitting into it needs an explicit twist stated in the first two sentences. A theme with 0-1 talks adjacent to the active speaker's expertise is a gap. Report both lists with counts.

## 6. Write back to the bank

After research, offer to persist findings using the templates in `bank/README.md`. Unpersisted research is wasted effort next cycle. Record the retrieval date on every entry since schedules and view counts drift.

## 7. Trend research

Choose sources for the active speaker's domain. The following are examples for software/AI; use equivalent scholarly, practitioner, or industry sources in other fields:

1. **Trendalyzer MCP** when connected: purpose-built, use it first.
2. **Consecutive conference schedules**: the strongest lagging confirmation. Diff track lists and theme clusters between editions (EU vs. NA, this year vs. last). A count increase or first appearance is evidence of changing programming; it does not by itself establish a peak or a rising trend.
3. **AI Engineer channel recency**: what the last 30 days of uploads cover, and which recent uploads have unusual view velocity for their age.
4. **Hacker News**: search the trend term; note first-appearance date, comment volume, and tone shift (excitement to backlash marks the peak).
5. **GitHub trending and release notes** from Anthropic, OpenAI, MCP spec repo, and the Agentic AI Foundation projects.

Assess trajectory, not heat. The CFP lead-time rule: whatever peaks at submission time is likely stale by talk day, so score topics by where they'll be at the event date. When a wave is cresting, the durable submission is either the rising successor or the persistent layer underneath (identify that durable layer from the active speaker's domain and evidence).

Snapshot every scan to `bank/trends/YYYY-MM-trends.md` with the date and evidence.

Keep public observations in the shared bank and speaker-specific angle tests or strategy in the active profile. Attribute interpretations separately from captured facts. Verify time-sensitive dates and facts live before recommending action.
