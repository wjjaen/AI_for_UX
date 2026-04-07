# PROMPTS.md
## Prompt Library — AI-Augmented Design

A curated, reusable prompt library organized by task. All prompts are optimized for Claude, Figma Make, Stitch, and Antigravity. Replace bracketed variables before use. Add new prompts at the bottom of each section as you develop them.

**Prompt Quality Rules:**
- Always include: role context, user/product context, and desired output format
- Be specific about tone, audience, and constraints
- The "80% there" principle: prompts should get you a strong first draft, not perfection

---

## 1. Research Brief & Framing

### Frame a Research Brief
```
Act as a senior UX research strategist.
Project: [name]
Product type: [app / web / feature]
Target user: [description]
Business goal: [what the business needs to decide]

Output:
1. A tight problem statement (1–2 sentences)
2. 3 answerable research questions
3. Recommended research method with rationale
4. Draft success criteria
5. One key assumption to pressure-test
```

### Sharpen Existing Research Questions
```
Review these research questions for rigor: [paste questions]
Flag any that are: too broad, leading, multi-part, or answerable without research.
Rewrite each flagged question. Explain the change in one sentence.
```

### Competitive Landscape Scan
```
Act as a UX and product strategist.
Analyze [competitor or market space] from a user experience perspective.
Output:
1. Core user flows (how users accomplish their main job)
2. UX strengths (what they do well)
3. Friction points (where users likely struggle)
4. Positioning gaps (underserved needs)
5. One insight I should apply to [my product]
Format as a structured table + 1 paragraph of strategic implication.
```

---

## 2. Persona & User Modeling

### Create a UX Persona from Research Data
```
Based on these research notes: [paste notes or themes]
Create a UX persona with:
- Name, role, age, context (realistic, not stereotypical)
- Top 3 goals (what they want to achieve)
- Top 3 pain points (with root causes, not just symptoms)
- Key behaviors (what they actually do, not what they say)
- A representative quote in their voice
- What success looks like for this person
Flag anything assumed vs. grounded in the data.
```

### Refine an Existing Persona
```
Here is an existing persona: [paste persona]
And here are new research findings: [paste findings]
Update the persona to reflect the new data.
Highlight what changed and why.
Keep it grounded — remove anything no longer supported.
```

### Generate User Journey Map (Current State)
```
Create a current-state journey map for [persona name] trying to [accomplish goal].
Map across these stages: [Awareness / Consideration / Onboarding / Regular Use / Drop-off — or customize]
For each stage include:
- Actions (what they do)
- Thoughts (what they're thinking)
- Emotions (frustrated / neutral / delighted — use a scale)
- Pain points
- Opportunities for design intervention
Output as a structured table.
```

---

## 3. Ideation & Concept Design

### Generate Design Concepts
```
I'm designing [product/feature] for [persona].
Their biggest pain point: [description]
Business goal: [description]
Constraints: [technical / brand / time / budget]

Generate 3 distinct design concepts. For each:
1. Concept name and core idea (1 sentence)
2. Key interaction or feature
3. Why this solves the pain point
4. Trade-off vs. the other concepts
5. Best used when: [context]
```

### HMW Question Generator
```
Convert these research insights into "How Might We" questions: [paste insights]
Rules: Each HMW should be open enough to inspire multiple solutions, but specific enough to guide direction.
Output: One HMW per insight. Sort by potential user impact (highest first).
```

### Feature Prioritization
```
Here is our feature list for [product]: [paste list]
Score each feature:
- User impact: 1–5 (5 = critical to user success)
- Business value: 1–5 (5 = directly drives revenue or retention)
- Implementation effort: 1–5 (5 = hardest / most time)

Calculate a priority score: (User Impact + Business Value) / Effort
Output as a ranked table. Flag top 5 for MVP. Flag anything high effort / low impact for cutting.
```

---

## 4. Prototyping — Stitch & Figma Make

### Stitch — Screen Generation Prompt
```
Create a [screen type, e.g., onboarding welcome screen] for [product name].
User: [persona description]
User goal on this screen: [what they need to accomplish]
Key UI elements: [list them]
Tone / brand: [minimal / friendly / bold / professional]
This screen comes after: [previous screen]
This screen leads to: [next screen]
Accessibility: Sufficient contrast, readable font sizes, touch-friendly targets.
```

### Stitch — User Flow Prompt
```
Design a complete [flow name, e.g., onboarding flow] for [product name].
User: [persona]
Flow goal: [what the user achieves by completing this flow]
Steps: [list the key steps, e.g., 1. Welcome, 2. Goal setting, 3. Profile setup, 4. Dashboard]
For each step include the primary action, key UI elements, and a success state.
Flag any step where users are likely to drop off and suggest a friction-reduction solution.
```

### Figma Make — Component Generation
```
Generate a [component type] component for [product name].
Context: [describe where/how it's used]
Must include: [list required elements]
States needed: default, hover, active, disabled, error
Style: [describe visual direction or link to design system tokens]
Accessibility requirements: [WCAG AA minimum, touch target 44px min]
```

---

## 5. Microcopy & UX Writing

### Onboarding Copy
```
Write onboarding copy for [screen name] in [product name].
User: [persona — their goal, emotional state at this point in the flow]
Screen purpose: [what the user needs to understand or do]
Tone: [empowering / friendly / minimal / professional]
Word limit: [e.g., headline 6 words max, body 2 sentences max]
Avoid: jargon, passive voice, anything that creates anxiety or confusion.
```

### Error Message Copy
```
Write error message copy for [error type] in [product name].
What went wrong: [technical description of the error]
What the user was trying to do: [context]
Tone: [calm / helpful / non-blaming]
Output: 
1. Error headline (clear, not alarming)
2. Body copy (explain what happened + what to do next)
3. CTA button label
Two versions: one concise (mobile), one with more context (desktop/web).
```

### CTA Copy Variants
```
Write 5 CTA button label options for [action] in [product name].
Context: [where this button appears, what it triggers]
User's goal at this point: [description]
Tone range: from [neutral/functional] to [motivational/urgent]
Avoid: "Submit", "Click here", "Next" — make it action + outcome specific.
```

### Microcopy — Empty States
```
Write empty state copy for [feature/screen] in [product name].
Scenario: User has [just signed up / completed all tasks / no data yet]
Tone: [encouraging / helpful / light]
Output:
1. Headline (acknowledge the state without negativity)
2. Body (1–2 sentences: context + what to do)
3. CTA (action-oriented)
```

---

## 6. User Flow Optimization & Debugging

### Full Flow Review
```
Evaluate the [flow name] flow for [product name] from the user's emotional journey.
User: [persona]
Flow steps: [list them]
Identify:
1. Steps with the highest cognitive load
2. Steps most likely to cause drop-off and why
3. Moments where motivation could be reinforced
4. Copy or label changes that would reduce friction
Output: Annotated flow table with specific, actionable fixes for each problem step.
```

### Single Screen Audit
```
Audit this screen for usability issues: [describe screen or paste screenshot description]
Product: [name]
User goal on this screen: [description]
Check for:
1. Clarity of primary action
2. Information hierarchy
3. Copy clarity (reading level, tone)
4. Potential confusion points
5. Accessibility concerns
Output: Prioritized list of issues with specific fix recommendations.
```

---

## 7. Research Synthesis

### Transcript → Themes
```
Analyze this user interview transcript: [paste — remove PII first]
Output:
1. Top 5 themes with supporting evidence (paraphrased quotes)
2. Key pain points (ranked by severity)
3. Moments of delight or positive behavior
4. Surprising or unexpected findings
5. 3 design implications
Format as a structured table.
```

### Multi-Session Synthesis
```
I conducted [N] user interviews. Here are the summarized notes: [paste]
Synthesize:
1. Top 3 themes appearing in 3+ sessions (with frequency count)
2. Top pain points ranked by frequency AND severity
3. Behavioral patterns (observed actions, not self-reported preferences)
4. One insight that challenges current assumptions
5. Design priorities in rank order with rationale
```

### Insight → Action Table
```
Convert these research insights into a design action plan: [paste insights]
For each insight:
- State the insight (clear, evidence-based)
- Recommended design action (specific)
- Effort: Quick win / Medium lift / Big bet
- Owner: Design / Product / Engineering / Content
Output as a table. Sort by impact-to-effort ratio.
```

---

## 8. Stakeholder Communication

### Executive Summary (Stakeholder-Ready)
```
Here are my research/design findings: [paste]
Write an executive summary for a [VP / C-suite / client] audience.
Format:
- 3 bullet key findings (plain language, outcome-focused)
- Business implication for each finding (1 sentence)
- 3 recommended actions in priority order
- Risk of inaction (1 sentence)
Tone: Direct, confident, non-defensive. No jargon.
```

### Design Decision Rationale
```
I made this design decision: [describe decision]
The alternatives I considered were: [list alternatives]
The user research that informed this: [describe evidence]
Write a design rationale document for developer/stakeholder handoff.
Include: decision, alternatives considered, research evidence, trade-offs acknowledged, and any open questions.
```

---

## 9. Antigravity (Google) — Workspace-Integrated Research

Use Antigravity when research data lives in Google Workspace — Docs, Sheets, Drive, or Meet recordings. These prompts are designed for Antigravity's ability to pull across connected Google data sources.

### Synthesize Research Across Google Drive Files
```
Search my Drive for documents related to [project name or topic].
Summarize the key findings across all relevant files.
Identify: 1) Common themes, 2) Conflicting data points, 3) Gaps not yet addressed.
Output: A synthesis table with source file references.
```

### Extract Insights from a Google Doc Interview Transcript
```
Open [document name or link].
This is a user interview transcript for [project name].
Extract:
1. Top 3 pain points with direct evidence
2. Key behaviors observed (what they do, not just what they say)
3. Moments of delight or positive reaction
4. One unexpected finding
5. 3 design implications
Format as a structured table.
```

### Analyze Survey Data from Google Sheets
```
Open [sheet name or link].
This is survey data from [N] respondents for [project name].
Analyze:
1. Top 3 patterns or trends in the responses
2. Any surprising outliers worth noting
3. Segments that responded differently (if demographic columns exist)
4. Draft 3 insight statements from the data
5. Recommend the single most important design implication
```

### Cross-Reference Research Against Design Decisions
```
I have research findings in [Drive doc/link] and a current design spec in [Drive doc/link].
Compare them:
1. Which design decisions are well-supported by the research?
2. Which decisions lack research backing?
3. Are there research findings not yet reflected in the design?
4. What's the highest-risk gap between what users need and what we've designed?
```

### Meeting Notes → Action Items (Google Meet / Docs)
```
Open the notes from [meeting name / date] in my Drive.
Extract:
1. Key decisions made
2. Open questions or unresolved items
3. Action items with owners (if named)
4. Any design or research implications
Format as a structured action log I can paste into Notion or a Figma cover page.
```

### Build a Research Repository Index
```
Search my Drive for all documents tagged or titled with [project name or research keywords].
Create an index of research assets including:
- Document name
- Date (if visible)
- Research method (interview / survey / usability test / secondary research)
- Key topic or finding (1 sentence)
- Status: current / outdated / needs review
Output as a table I can use as a living research repository.
```

---

## Prompt Log — Personal Additions

*Use this section to log prompts you've developed and tested. Format: Task | Prompt | Tool | Rating (1–5) | Notes*

| Task | File Location | Tool | Rating | Notes |
|---|---|---|---|---|
| [Add yours here] | | | | |
