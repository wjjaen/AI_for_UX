# HANDOFF.md
## Design & Research Handoff Frameworks

Everything you need to close a project phase cleanly — from developer-ready design annotations to stakeholder research readouts. Built for speed and clarity, not ceremony.

---

## 1. Design Handoff to Development

### Handoff Readiness Checklist
Before marking any design ready for development:

**Screens & States**
- [ ] All screens accounted for (including edge cases)
- [ ] Every interactive element has all states: default, hover, focus, active, disabled, error, loading, empty
- [ ] Empty states designed (no data, first-time user, error)
- [ ] Responsive breakpoints defined (mobile, tablet, desktop — as applicable)
- [ ] Dark mode / light mode covered (if required)

**Components & Specs**
- [ ] Components named consistently and organized in Figma
- [ ] Design tokens used (not hardcoded values) — colors, spacing, typography
- [ ] Touch targets minimum 44×44px
- [ ] Contrast ratios checked (WCAG AA minimum: 4.5:1 text, 3:1 UI components)
- [ ] Font sizes, weights, and line heights specified

**Interactions & Behavior**
- [ ] Interaction annotations added to complex flows
- [ ] Animation/transition specs documented (duration, easing)
- [ ] Conditional logic explained (if X then show Y)
- [ ] API dependencies flagged for engineering

**Content**
- [ ] All copy finalized (no Lorem Ipsum)
- [ ] Character limits noted for dynamic content fields
- [ ] Error messages and validation copy included
- [ ] Tooltips and helper text included

---

### AI Assist — Annotation Generator
```
I have a [screen name] screen in Figma with these elements: [list elements]
Write developer handoff annotations for each element. Include:
- Behavior description (what it does)
- All states: default, hover, active, disabled, error, loading
- Any conditional logic ("only shown when X")
- Content rules (character limits, dynamic vs. static)
- Accessibility notes (ARIA labels, keyboard behavior)
Language level: Front-end developer. Precise, not verbose.
```

### AI Assist — Interaction Spec Writer
```
Describe the interaction spec for this component: [describe component]
Product: [name]
Behavior: [what triggers it, what happens, what follows]
Write a concise interaction spec covering:
1. Trigger (what causes the interaction)
2. Animation (type, duration, easing — or "none")
3. State change (what visually changes)
4. Success/error handling
5. Edge cases to handle
Format for a Figma annotation or Notion doc.
```

---

## 2. Research Handoff to Stakeholders

### Research Readout Structure
Use this structure for any research findings delivery — interview synthesis, usability test results, or survey analysis.

```
1. TL;DR (3 bullets — the most important things they need to know)
2. What we did (method, participants, timeline — 3 sentences max)
3. Key findings (3–5 insights, each with evidence)
4. Design implications (insight → action table)
5. Recommended next steps (specific, owned, time-bound)
6. Appendix (transcripts, screener, raw data — for those who want to dig)
```

### AI Assist — Research Readout Generator
```
Here are my research findings: [paste themes, quotes, observations]
Audience: [VP / client / product team / engineering]
Write a research readout using this structure:
1. TL;DR — 3 bullets, outcome-focused, plain language
2. What we did — 2–3 sentences (method, N, timeline)
3. Key findings — 3–5 insights with one paraphrased evidence quote each
4. Design implications — table: Insight | Design Action | Effort | Owner
5. Recommended next steps — 3 actions, each with a suggested owner
Tone: Direct and confident. No jargon. Built for a 5-minute read.
```

### AI Assist — Executive Summary (60-Second Version)
```
Compress these research findings into a 60-second verbal summary for [audience]: [paste findings]
Format:
- Opening: the single most important thing we learned
- Supporting: 2 findings that back it up
- So what: one recommended action
- Closing: what happens if we don't act
Write as spoken word — natural, not bullet-point reading.
```

---

## 3. Design Decision Documentation

### Design Rationale Template
Use when documenting why a design decision was made — for future reference, stakeholder challenges, or team onboarding.

```
Decision: [what was decided]
Date: [when]
Decision maker(s): [who]

Options considered:
1. [Option A] — [brief description + trade-off]
2. [Option B] — [brief description + trade-off]
3. [Option C, if applicable]

Evidence that informed this:
- User research: [what users said or did]
- Business requirement: [what the business needed]
- Technical constraint: [if applicable]

Decision rationale: [why this option, in 2–3 sentences]

Trade-offs acknowledged: [what we gave up or accepted]

Open questions: [anything still unresolved]

Revisit trigger: [what would cause us to reconsider this decision]
```

### AI Assist — Design Rationale Writer
```
I made this design decision: [describe decision]
Alternatives I considered: [list them]
Research that informed it: [paste evidence]
Business or technical constraints: [describe]

Write a design rationale document using the standard template.
Tone: Confident but not defensive. Acknowledge trade-offs honestly.
This will be read by: [product team / client / future designers on the project]
```

---

## 4. Stakeholder Presentation Handoff

### Presentation Structure (Design Review or Project Closeout)
| Section | Content | Length |
|---|---|---|
| Context | What we set out to solve | 1 slide |
| Process | How we got here (methods used) | 1–2 slides |
| What we learned | Key insights from research | 2–3 slides |
| What we designed | Solution walkthrough | 3–5 slides |
| Evidence | Test results, metrics, validation | 1–2 slides |
| Next steps | What happens now | 1 slide |

### AI Assist — Presentation Narrative Builder
```
I need to present [project name] to [audience].
Here is what we did and found: [paste summary]
Key design decisions: [list them]
Results or validation: [test findings, metrics, or qualitative evidence]

Write a presentation narrative for [N] slides.
For each slide: title, 3-bullet content, and one visual description (chart / screenshot / quote).
Tone: [strategic / technical / storytelling — pick one]
Audience's biggest question: [what they most want to know]
Close with a clear ask or next step.
```

---

## 5. Figma File Organization for Handoff

### File Structure Standard
```
📁 [Project Name]
  ├── 📄 Cover (project name, version, date, status)
  ├── 📄 Index (page map with descriptions)
  ├── 📄 Design System / Tokens (colors, type, spacing, components)
  ├── 📄 User Flows (high-level flow diagrams)
  ├── 📄 [Feature Name] — Screens
  ├── 📄 [Feature Name] — Screens (repeat per feature)
  ├── 📄 States & Edge Cases
  ├── 📄 Annotations & Specs
  └── 📄 Archive (deprecated screens — never delete, just move here)
```

### Naming Conventions
- Screens: `[Feature]/[Screen Name]/[State]` — e.g., `Onboarding/Goal Setting/Error`
- Components: `[Category]/[Name]/[Variant]` — e.g., `Button/Primary/Disabled`
- Colors: `[Role]-[Modifier]` — e.g., `brand-primary`, `feedback-error`, `neutral-300`

### AI Assist — Figma Handoff Notes Generator
```
Write a Figma handoff summary note for [feature name].
What this feature does: [description]
Key screens included: [list]
Known limitations or open questions: [list]
What dev needs to know before building: [technical notes]
Accessibility requirements: [list]
Dependencies: [APIs, other features, content from other teams]
Format as a Figma cover page note — clear, scannable, under 200 words.
```

---

## 6. Handoff Anti-Patterns

| Anti-Pattern | Impact | Fix |
|---|---|---|
| Handing off screens without states | Dev has to guess — adds back-and-forth | Always spec all interactive states |
| No empty or error states | Broken production experience | Design these before handoff, not after |
| Hardcoded values instead of tokens | Design system debt | Use token variables in Figma from the start |
| Verbal-only design rationale | No record when challenged | Document every non-obvious decision |
| Research findings in a slide deck no one reads | Insights get ignored | Pair the deck with a 1-page TL;DR and a verbal walkthrough |
| "Dev can figure out the interactions" | Wrong assumptions baked into code | Annotate anything with motion, logic, or conditional behavior |
