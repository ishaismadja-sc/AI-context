# People Dynamics Framework

> Operational guide for building, updating, and maintaining people profiles in people-dynamics.md.
> Invoked via `!dynamics [person]`, `!dynamics [channel]`, or `!dynamics all`.
> Built April 2026 from @ContextResearcher domain brief (organizational network analysis, LIWC-22 linguistic analysis, Goffman frontstage-backstage theory, ICD 203 confidence calibration, Korn Ferry behavioral coding).
> Agents involved: @Scout (internal retrieval), @JP (identity diagnostics, bias audit, framing guide), @PromptArchitect (profile quality review on request).

---

## What This Is

A structured methodology for building behavioral profiles of colleagues from Slack communication signals. Profiles serve all downstream agents - meeting prep, feedback framing, political navigation, coalition analysis, development planning.

**What this is NOT:** A psychometric assessment, a performance evaluation, or surveillance. Profiles are hypotheses about operating style and relational dynamics, built from observable behavior, calibrated for confidence, and subject to revision.

---

## Invocation

`!dynamics [person]` - New profile or full refresh of an existing profile
`!dynamics [person] - refresh` - Lightweight update (recent signals only, no full rebuild)
`!dynamics [channel]` - Channel dynamics analysis (Part D style)
`!dynamics all` - Full sweep of all profiles (quarterly)

### New Profile vs. Refresh

**New profile:** Full pipeline. Use when adding someone to people-dynamics.md for the first time, or when the existing profile is >90 days old and the relationship has shifted materially.

**Refresh:** Scan last 30 days of DMs and relevant channels. Update only sections where new signal exists. Append to diagnostic episodes if something notable occurred. Don't rewrite stable sections. Research budget: 50% of new profile.

---

## Confidence Calibration

Every profile element gets a confidence marker. This is non-negotiable - it's how downstream agents know what to trust.

### Evidence Tiers

| Tier | Source type | Confidence ceiling | Example |
|------|-----------|-------------------|---------|
| **Tier 1: Structural metadata** | Message counts, channel membership, response timing, network position | High | "Posts 3x more in DMs than public channels" |
| **Tier 2: Aggregated content** | Patterns across 50+ messages, recurring behaviors, consistent framing | Moderate-High | "Consistently leads with data before recommendations" |
| **Tier 3: Episode-based** | Specific diagnostic interactions, notable threads, revealing moments | Moderate | "In the CHAOS event thread, responded with 'good callout' then no follow-up" |
| **Tier 4: Single observation** | One message, one reaction, one absence | Low | "Used a thumbs-down emoji on the proposal" |
| **Tier 5: Inferred** | No direct source, pattern-matched from adjacent signals | Flag explicitly | "Likely frustrated based on declining message frequency" |

### Confidence Language (adapted from ICD 203)

| Term | Meaning | When to use |
|------|---------|-------------|
| **Established** | 10+ supporting observations across multiple contexts | Core operating mode, well-documented relationship patterns |
| **Assessed** | 3-9 supporting observations with some consistency | Most behavioral pattern claims |
| **Preliminary** | 1-2 observations, plausible but thin | New profiles, emerging patterns |
| **Hypothesized** | Inferred from adjacent signals, no direct observation | Trait mappings, motivation hypotheses |

### Minimum Signal Thresholds

| Profile element | Minimum data required | Below threshold action |
|----------------|----------------------|----------------------|
| Operating mode | 30+ messages across 2+ contexts | Flag as "preliminary read" |
| Relationship quality | 20+ bilateral DMs | Flag as "insufficient DM history" |
| @JP diagnostic | Operating mode + relationship quality established | Produce observational summary only, defer diagnostic |
| Key biases | 3+ episodes demonstrating the bias | List as "watch for" not "established pattern" |
| Framing guide | Operating mode + 2+ diagnostic episodes | Generic guidance only |

### Profile Confidence Rating

Every completed profile gets an overall confidence rating in its header comment:

```
<!-- Signal density: High | Moderate | Low. Last verified: [date] -->
```

- **High:** MGMT assessment data available + 100+ DMs + regular channel activity + 3+ diagnostic episodes
- **Moderate:** 50+ DMs + channel activity + 1-2 diagnostic episodes (OR assessment data + thin DM history)
- **Low:** <50 DMs, limited channel visibility, no assessment data. Flag as provisional.

---

## Phase 0: Clarifying Questions (before any research)

Parse the invocation first. Only ask what's not already provided.

**Questions (ask only what's needed):**

1. **Assessment data.** Do you have MGMT assessment scores (Top 5/Bottom 5, MBTI) for this person? This determines Part A vs. Part B profile depth.
2. **Relationship context.** How frequently do you interact? DMs, meetings, channels? (Calibrates expected signal volume.)
3. **Specific concerns.** Is there a reason you're profiling this person now? A friction, a decision, an upcoming conversation? (Focuses the research on what matters.)

If the person is already in people-dynamics.md, skip question 2 - load the existing profile instead and ask: "Full rebuild or refresh?"

---

## Phase 1: Load Context

### Step 1: Read people-dynamics.md

If updating an existing profile, load the current version. Note what's there, what's thin, what might be stale.

If creating a new profile, read Part E (cross-cutting dynamics) to understand where this person fits in the existing architecture.

### Step 2: Read scout-sources.md

Identify: the person's Slack user ID, relevant channels for their domain, related people's IDs (their reports, their friction partners, their manager).

### Step 3: Determine profile section

| Condition | Section | Profile depth |
|-----------|---------|--------------|
| Sara's direct report, MGMT assessment available | Part A | Full: attribute profile, incarnations, operating mode, relationship quality, diagnostic episodes, public channel behavior, key biases, framing guide |
| Sara's direct report, NO assessment data | Part A (observational) | Reduced: operating mode, relationship quality, diagnostic episodes, public channel behavior, key biases (flagged as observed), framing guide. No attribute profile or incarnations. |
| Ishai's direct report or key operational relationship | Part B | Standard: role, operating style, relationship with Ishai, @JP diagnostic, key biases/risks, how to work with them |
| External partner, board member, infrequent contact | Part B (provisional) | Minimal: role, operating style, relationship context, provisional framing guide. Flag as low-confidence. |

---

## Phase 2: Research Pipeline

Use @Scout methodology: load the map, classify and route, search iteratively, follow chains, attribute and rank findings.

### DM Loading Protocol

Follow the same protocol as prep-framework.md:
- **Set `oldest` to 90 days before today** for new profiles (vs. 30 days for prep). Longer window = richer behavioral sample.
- **Set `limit` to 200** for new profiles, 50 for refresh.
- If DMs appear to end months ago, check group DMs: `slack_search_public_and_private` with both user IDs.
- Verify bidirectional communication. One-directional DMs are a signal in themselves.

### Research Sequence

**1. DM History (highest-value source)**
- Read Ishai's DMs with the person (DM Loading Protocol)
- Note: topic distribution, emotional register, who initiates, response patterns, what they come to Ishai for vs. what Ishai goes to them for
- Identify 2-5 diagnostic episodes - interactions that reveal operating mode under pressure, conflict, or ambiguity

**2. Public Channel Behavior**
- Read their recent posts in #sc-live-leadership and #sc-core-leadership (if they post there)
- Read their primary domain channels (identified from scout-sources.md)
- Note: posting frequency, substance vs. logistics ratio, who they respond to, who responds to them, credit/blame patterns, vulnerability vs. command register

**3. Frontstage-Backstage Gap Analysis**
- Compare DM register (tone, vulnerability, directness) with public channel register
- A large gap signals impression management, low psychological safety, or political calculation
- A small gap signals authenticity or disengagement
- **Cultural calibration required:** Finnish colleagues may show small gaps due to cultural restraint, not authenticity. Israeli colleagues may show large gaps due to cultural directness norms in private vs. professional norms in public English-language channels.

**4. Network Position (from behavioral signals)**
- Who do they DM most? (Check if accessible)
- Which channels are they most active in?
- Who do they @mention? Who @mentions them?
- Are they a connector (bridges groups), a peripheral specialist (deep but narrow), or a central hub?

**5. Targeted Deep Dives**
- Follow thread chains from diagnostic episodes
- Fetch linked documents referenced in notable messages
- Check for their messages in channels Ishai doesn't typically monitor

### Research Budget

| Profile type | Tool call budget | Minimum DM messages to read |
|-------------|-----------------|---------------------------|
| New Part A profile | 15-25 calls | 100+ |
| New Part B profile | 10-20 calls | 50+ |
| Refresh | 5-10 calls | Last 30 days |
| Provisional (thin signal) | 5-8 calls | Whatever's available |

---

## Phase 3: Behavioral Coding

After research, code findings into profile elements. Use this taxonomy to translate raw observations into structured profile content.

### Communication Signature (Tier 1 - metadata-derived, HIGH confidence)

| Signal | What it reveals | How to measure from Slack |
|--------|----------------|-------------------------|
| Message volume | Engagement level, communication style | Count messages per week across channels and DMs |
| Channel vs. DM ratio | Public comfort, political awareness | Compare public posts to DM messages |
| Initiation ratio | Agency, dependency, power dynamics | Who starts conversations more often |
| Response latency | Engagement, workload, relationship priority | Time between message and response (rough) |
| Message length | Processing style, detail orientation | Average message length in words |
| Time-of-day patterns | Work rhythm, timezone adaptation | When they post |

### Behavioral Patterns (Tier 2-3 - content-derived, MODERATE confidence)

Code recurring patterns using these dimensions (adapted from Korn Ferry competency clusters):

| Dimension | What to look for in Slack | Profile section it feeds |
|-----------|--------------------------|------------------------|
| **Decision style** | Speed of position-taking, evidence requirements, how they handle ambiguity | Operating mode |
| **Conflict approach** | Public vs. private disagreement, directness, blame/credit patterns | What to watch, framing guide |
| **Information sharing** | Proactive updates, information hoarding, transparency | @JP diagnostic |
| **Help-seeking** | Asks questions publicly vs. privately, frames asks as collaboration vs. need | Relationship quality |
| **Emotional register** | Vulnerability, humor, warmth, detachment, formality | Operating mode, framing guide |
| **Power signaling** | "I" vs. "we" vs. "the team" language, credit attribution, deference patterns | @JP diagnostic |
| **Stress behavior** | What changes under pressure - shorter messages, channel withdrawal, increased DMs, blame displacement | What to watch, risk profile |

### Linguistic Markers (Tier 2 - applied qualitatively, MODERATE confidence)

Don't run LIWC software. Instead, apply these validated findings as a qualitative reading lens:

| Marker | Research basis | What to look for |
|--------|---------------|-----------------|
| First-person pronoun frequency | Kacewicz et al. 2014 - lower-status individuals use more "I/me/my" | Heavy "I" usage in DMs but "we" in public = impression management |
| Tentative language | Pennebaker - "maybe," "I think," "not sure" correlate with lower confidence/power | Sudden increase = anxiety or new territory |
| Certainty language | Pennebaker - "absolutely," "clearly," "obviously" | Overuse may signal overcompensation or defensiveness |
| Negative emotion words | Pennebaker - increase under stress | Track over time, not absolute level |
| Question frequency | Edmondson - questions signal psychological safety | Who asks questions publicly vs. never |

**Critical constraint:** These markers are interpretive lenses, not diagnostic instruments. A single message with "I think maybe" is meaningless. A persistent pattern across 50+ messages is a signal worth noting. Always code as Tier 2 or lower.

---

## Phase 4: @JP Diagnostic

After behavioral coding is complete, @JP produces the identity-level interpretation. This is where raw behavioral observations become a diagnostic profile.

### What @JP Adds

| Element | What @JP provides | What @JP does NOT provide |
|---------|------------------|--------------------------|
| Identity dynamics | Which professional identity is at stake, how they protect it | Therapy-level personality assessment |
| Power positioning | How they navigate the flat structure, where they derive authority | Moral judgment about their politics |
| Defensive patterns | What anxieties they manage, which mechanisms they use | Pathologizing normal behavior |
| Relationship diagnostic | Quality and nature of the relationship with Ishai, risks, dynamics | Relationship advice |
| Cognitive biases | 2-3 biases most actively shaping their behavior, with evidence | Comprehensive bias inventory |

### @JP Must Cross-Reference

- Ishai's own biases (from agent-registry: User's Known Cognitive Patterns) - are any distorting this profile?
- Cultural baselines - Finnish communication norms ≠ Israeli norms ≠ international-English norms
- Position effect - the COO is profiling direct reports and peers; impression management is maximal

### The Profiler Bias Check

Before finalizing any profile, @JP runs this checklist on the profiler (Ishai), not the subject:

| Bias | Risk | Check |
|------|------|-------|
| Halo effect | Warm communicators get warmer profiles | Is the positive framing supported by behavioral evidence, or by how the person makes Ishai feel? |
| Communication-volume bias | Frequent messagers get richer, more sympathetic profiles | Compare profile depth to signal volume. Flag if someone with 200 DMs has a richer profile than someone with 50 who may contribute more. |
| In-group bias | Hebrew speakers, Israel-based colleagues | Are comparable behaviors interpreted more charitably for in-group members? |
| Recency bias | Recent interaction colors the whole profile | Check whether diagnostic episodes span time or cluster in one period |
| Fundamental attribution error | Attributing behavior to personality vs. situation | For every behavioral pattern, name the situational explanation too |

---

## Phase 5: Profile Assembly

### Profile Templates

#### Part A Profile (with MGMT assessment)

```
## [Section#]. [Name] - [Title]

**Attribute profile**: Top 5: [trait (score)], ... Bottom 5: [trait (score)], ... MBTI: [type].

**Incarnations**: Best: [1 sentence]. Worst: [1 sentence].

**Operating mode**: [Archetype name]. [2-3 sentences on how they operate].

**Relationship quality**: [2-4 sentences on the dynamic with Ishai, grounded in diagnostic episodes].

**[Diagnostic episode label]**: [Specific interaction that reveals a pattern. Include what happened, what it revealed, and what it means for working with them.]

**Public channel behaviour**: [1-3 sentences on how they show up in leadership/domain channels].

**Key biases**: [2-3 biases with brief context].

**Framing guide**: [3-5 direct instructions for how to communicate with this person].
```

#### Part A Profile (observational - no assessment data)

```
## [Section#]. [Name] - [Title]
<!-- Signal density: [High/Moderate/Low]. No MGMT assessment. Last verified: [date] -->

**Operating mode**: [Archetype name]. [2-3 sentences].

**Relationship quality**: [2-4 sentences].

**[Diagnostic episode label]**: [Specific interaction analysis].

**Public channel behaviour**: [1-3 sentences].

**Key biases**: [2-3 biases, flagged as "observed patterns" not assessment-confirmed].

**Framing guide**: [3-5 direct instructions].
```

#### Part B Profile

```
## [Section#]. [Name] - [Title]
<!-- Signal density: [High/Moderate/Low]. Last verified: [date] -->

**Role**: [1-2 sentences].

**Operating style**: [2-3 sentences on how they work].

**Relationship with Ishai**: [2-3 sentences].

**@JP diagnostic**: [3-5 sentences on identity dynamics, power positioning, risks].

**Key biases/risks**: [2-3 items].

**How to work with them**: [3-5 direct instructions].
```

#### Provisional Profile (thin signal)

```
## [Section#]. [Name] - [Title]
<!-- Signal density: Low. PROVISIONAL - insufficient data for full diagnostic. Last verified: [date] -->

**Role**: [1-2 sentences].

**Operating style**: [1-2 sentences, flagged as preliminary].

**Relationship context**: [How Ishai interacts with them, frequency, channel].

**Provisional framing guide**: [2-3 generic guidelines based on available signal].

**Data gaps**: [What would be needed for a full profile - more DMs, channel observation, in-person interaction].
```

### Writing Standards

- **Observation before interpretation.** For every interpretive claim, the supporting observation must appear first or be traceable.
- **Specific over general.** "She led with data in 3 of 4 disagreement threads" beats "She's data-driven."
- **Diagnostic episodes earn their space.** Each episode must reveal something about operating mode, not just report an interaction.
- **No moral judgment.** "Low Empathy" is a profile trait, not a character flaw. "Routes around central systems" is a behavior, not a moral failing.
- **Cultural calibration.** Note when a behavior may reflect cultural norms rather than individual traits.

---

## Phase 6: Integration

After the profile is written:

### Update Part E (Cross-Cutting Dynamics)

Check whether the new profile changes any cross-cutting patterns:
- Does this person belong to the inner ring or boundary operators?
- Do they have a friction axis with anyone already profiled?
- Do they create a new information asymmetry or containment dynamic?
- Do they affect the thin error-correction pattern?

### Update Part D (Channel Dynamics) if Relevant

If the person is active in #sc-live-leadership or #sc-core-leadership, update the channel dynamics section.

### Flag Downstream Impacts

New profiles may affect:
- `prep-framework.md` - if the person is someone Ishai preps for regularly
- `weekly-checkin-framework.md` - if the person is in the weekly meeting room
- Agent prompts with hardcoded people context (check @Brand, @UA for Key Relationship Context sections)

---

## Maintenance Protocol

### Quarterly Full Sweep (`!dynamics all`)

- Re-scan all profiled people's DMs and channels (last 90 days)
- Flag profiles where behavior has shifted materially
- Update signal density ratings
- Check for stale diagnostic episodes (>6 months without new signal)
- Update Part E cross-cutting dynamics

### Event-Triggered Refresh

Refresh a profile immediately when:
- The person changes role, title, or reporting line
- A significant conflict or friction event occurs
- Ishai's relationship with them shifts notably
- They're about to be discussed in a strategic context (LRP, org design)

### Version Discipline

- Never overwrite diagnostic episodes - append new ones
- When updating "operating mode" or "@JP diagnostic," note what changed and why
- Update the `<!-- Last verified: [date] -->` comment on every touch
- Log significant profile changes in the Agent System Changelog (Notion)

---

## Anti-Patterns

| Don't | Do instead |
|-------|------------|
| Build a profile from <30 DMs and present it with the same weight as one built from 200 | Flag signal density. Produce a provisional profile when data is thin. |
| Attribute behavior to personality when situation explains it equally well | Name both explanations. "This could reflect low Persistence OR reflect Q4 workload." |
| Write the @JP diagnostic before completing behavioral coding | Observation first, interpretation second. Always. |
| Profile someone you rarely interact with and assume equal insight | Your profile of a frequent-DM person is structurally richer. Note the asymmetry. |
| Apply the same cultural baseline to Finnish and Israeli colleagues | Establish separate baselines. Finnish silence ≠ disengagement. Israeli directness ≠ aggression. |
| Let the halo effect from warm communicators produce warmer profiles | Run the profiler bias check (Phase 4) on every profile. |
| Present a LIWC-style linguistic reading as personality assessment | Linguistic markers are qualitative lenses, not diagnostic instruments. Tier 2 confidence maximum. |
| Skip Part E updates when adding a new profile | Every new person changes the system. Check cross-cutting dynamics. |
| Produce a profile without stating what you couldn't find | Data gaps are findings. "No public channel posts in 60 days" is as important as what they posted. |
| Rewrite stable sections during a refresh | Refresh mode updates what's new. Stable sections persist unless contradicted. |
| Copy the thin-slice approach from face-to-face to text | Ambady's thin-slice accuracy does not transfer to edited text communication. Text lets people curate. |
| Profile someone without checking your own biases first | The profiler bias check exists because your relationship system has documented thin error-correction. |
| Treat this as surveillance | These are working hypotheses for better collaboration, not dossiers. |

---

## People Context

**Do not hardcode people profiles in this framework.** All people data lives in `people-dynamics.md`. This framework defines HOW to build and maintain profiles, not WHAT the profiles contain. Slack IDs and channel mappings live in `scout-sources.md`.

---

## Notes for Execution

- **Hebrew DMs**: DMs with Maya (and potentially other Israeli colleagues) may be predominantly Hebrew. Note the language distribution as a signal, but don't exclude Hebrew messages from behavioral coding - tone, frequency, and structural patterns are readable even without full translation.
- **Group DMs**: Some relationships operate primarily through group DMs rather than bilateral DMs. If bilateral DM history seems thin, search for group DMs before concluding the relationship is thin.
- **Slack canvases**: Some 1:1 relationships have shared canvases in the DM channel. These are rich sources of relationship history and priority tracking.
- **External contractors**: Alexandra (EA) is external with no institutional identity. Profiles of external people should note this context - their communication patterns are shaped by different incentive structures.
- **Assessment data asymmetry**: Part A profiles WITH assessment data are structurally different from those without. Don't simulate assessment data - the absence is informative and downstream agents should know.
