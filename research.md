# RESEARCH.md
## AI-Augmented User Research Workflow

End-to-end research process from framing the brief to handing off findings. Optimized for speed without sacrificing rigor. Every phase includes AI-assisted steps using Claude, Miro/FigJam, and Antigravity.

---

## Phase 1 — PLAN: Frame the Research Brief

**Goal:** Define exactly what you need to learn, and why, before collecting a single data point.

### Research Brief Template
```
Project: [name]
Business question: [What decision does this research need to inform?]
User segment: [Who are we researching?]
Research questions (3 max):
  1.
  2.
  3.
Method: [interviews / survey / usability test / diary study]
Timeline: [dates]
Participants needed: [number + screener criteria]
Success criteria: [How will we know this research was useful?]
```

### AI Assist — Brief Sharpener
```
I need to run user research for [project]. Here's my initial brief: [paste draft]
Review it as a senior research strategist:
1. Are the research questions answerable and specific enough?
2. Is the method the right fit?
3. What critical questions am I missing?
4. What biases might skew results?
Output: Revised research questions + one risk flag.
```

### Common Research Question Mistakes to Avoid
- Too broad: "What do users think about our app?" → Too vague
- Leading: "Why do users love the onboarding?" → Assumes sentiment
- Multi-part: "What do users want and how often do they use it?" → Split these
- Solvable without research: "Should we use blue or green?" → Preference test, not research

---

## Phase 2 — RECRUIT: Find the Right Participants

**Goal:** Get the right people, not just any people.

### Screener Criteria Framework
- **Role/behavior:** What must they currently do or be?
- **Experience level:** Novice, regular, or power user?
- **Exclusions:** Competitors, internal employees, extreme outliers
- **Demographics:** Only include if directly relevant to the research question

### AI Assist — Screener Survey Generator
```
Write a participant screener survey for [project].
Target user: [description]
Must include: [key qualifying behaviors or traits]
Must exclude: [disqualifying factors]
Format: 6–8 questions, mix of multiple choice and short answer.
End with a consent + availability question.
```

### Sample Sizes (Quick Reference)
| Method | Recommended N | Why |
|---|---|---|
| Qualitative interviews | 5–8 | Saturation point for themes |
| Usability testing | 5 per user group | Uncovers ~85% of issues |
| Survey (quantitative) | 100+ | Statistical significance |
| Diary study | 10–15 | Longitudinal behavioral data |

---

## Phase 3 — COLLECT: Run Interviews & Surveys

**Goal:** Gather rich, unbiased data efficiently.

### Interview Plan Structure
1. **Intro** (5 min) — Build rapport, explain the session, get consent
2. **Context questions** (10 min) — Understand their world before diving in
3. **Core questions** (25 min) — Explore the research questions
4. **Task observation** (if prototype testing) (15 min)
5. **Debrief** (5 min) — "Is there anything important I didn't ask?"

### AI Assist — Interview Guide Generator
```
Write a user interview guide for [project].
Research questions: [list your 3 research questions]
User segment: [description]
Session length: [45 / 60 / 90 min]

Output:
- Intro script (neutral, non-leading)
- 5 warm-up context questions
- 8–10 core questions (open-ended, no leading language)
- 3 follow-up probes to dig deeper
- Closing script
```

### Best Practices for AI-Assisted Transcription
- Use **Otter.ai** or **Whisper** for auto-transcription
- Always review and clean transcripts before analysis — AI makes errors on names, jargon, and accents
- Tag speaker turns clearly: [MODERATOR] / [PARTICIPANT]
- Remove PII before feeding transcripts into any AI tool for analysis

### Data Ethics Checklist
- [ ] Informed consent obtained before recording
- [ ] Participants told how data will be stored and used
- [ ] PII removed from transcripts before AI analysis
- [ ] Data stored securely (not in public cloud folders)
- [ ] Participants can withdraw data upon request

---

## Phase 4 — ANALYZE: Synthesize Raw Data

**Goal:** Turn messy notes and transcripts into clear, prioritized insights.

### AI Assist — Rapid Synthesis (Transcript → Themes)
```
Here is a user interview transcript: [paste transcript — remove PII first]

Analyze it as a UX researcher:
1. List the top 5 recurring themes
2. Identify key pain points with direct evidence
3. Identify moments of delight or positive behavior
4. Flag any surprising or unexpected findings
5. Suggest 2–3 design implications

Format: Structured table with theme, evidence quote (paraphrased), and design implication.
```

### AI Assist — Multi-Interview Synthesis
```
I have conducted [N] user interviews. Here are the summarized notes from each: [paste]

Synthesize across all sessions:
1. Top 3 themes that appeared in 3+ sessions
2. Top 3 pain points by frequency and severity
3. Behavioral patterns (what users do, not just what they say)
4. One key insight that challenges our current assumptions
5. Recommended design priorities in rank order
```

### Affinity Mapping in Miro (AI-Assisted)
1. Paste raw notes as individual sticky notes in Miro
2. Use Claude to pre-cluster: "Group these observations into 5–7 themes: [paste notes]"
3. Use the AI clusters as a starting scaffold, then manually review and adjust
4. Name each cluster with an insight statement, not just a label (e.g., "Users lose motivation without visible progress" not just "Motivation")

### Insight Statement Formula
> **We discovered that** [observation] **which means** [implication] **so we should** [design direction].

---

## Phase 5 — SYNTHESIZE & SHARE: From Insights to Action

**Goal:** Communicate findings in a way that drives decisions, not just informs them.

### Research Readout Structure
1. **TL;DR** — 3 bullet executive summary (AI can draft this)
2. **Research context** — What we studied, who, how many
3. **Key findings** — 3–5 insights with evidence
4. **Design implications** — Insight → Action mapping
5. **Recommended next steps** — Specific, owned, time-bound
6. **Appendix** — Raw data, screener, full transcripts

### AI Assist — Executive Summary Generator
```
Here are my research findings: [paste findings]

Write an executive summary for a stakeholder presentation:
- 3 bullet key findings (plain language, no jargon)
- 1 sentence business implication for each finding
- 3 recommended actions in priority order
Tone: Direct, confident, non-defensive. This is for a VP-level audience.
```

### AI Assist — Insight → Action Mapping
```
Convert these research insights into a design action plan: [paste insights]

For each insight:
- State the insight clearly
- Describe the recommended design action
- Assign an effort level: Quick win / Medium lift / Big bet
- Suggest which team owns it: Design / Product / Engineering / Content
Output as a table.
```

### Prototype Testing Readout Template
For usability test findings, structure your readout as:
1. Test objectives & hypotheses
2. AI-assisted executive summary (use Claude to compress raw session notes)
3. Observational notes by flow (what worked / what didn't / suggested fix)
4. Usability scores (completion rate, ease of use, emotional response)
5. Insight clustering by theme
6. Design implications table
7. Next steps with owners and dates

---

## Research Anti-Patterns to Avoid

| Anti-Pattern | Why It's a Problem | Fix |
|---|---|---|
| Asking leading questions | Biases responses toward your hypothesis | Rewrite as open-ended: "Tell me about a time when..." |
| Recruiting only happy users | Creates survivorship bias | Screen for a range of experience levels |
| Treating AI synthesis as final | AI misses nuance, emotion, and context | Always review and edit AI-generated themes |
| Reporting what users said vs. what they did | Self-reported behavior is unreliable | Prioritize observed behavior over stated preference |
| Skipping the debrief | Miss critical context | Always end with "Is there anything important I didn't ask?" |
