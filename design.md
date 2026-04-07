# DESIGN.md
## AI-Augmented UX/UI Design Process

A phase-by-phase design framework with AI integration points, tool recommendations, and decision triggers. Built for advanced practitioners who already know the process — this is your AI-enhanced operating system.

---

## Phase 0 — Project Kickstart

**Goal:** Define the problem space, constraints, and success criteria before touching any design tool.

### Kickstart Checklist
- [ ] Problem statement defined (user + need + insight)
- [ ] Business goal aligned with design goal
- [ ] Target user segment identified (rough)
- [ ] Success metrics agreed on with stakeholders
- [ ] Constraints documented (time, tech, brand, budget)
- [ ] Research needed? → Go to `research.md`

### AI Assist — Project Brief Generator
Paste into Claude:
```
Act as a senior UX strategist. Help me frame a project brief for [project name].
Product type: [app / web / service / feature]
Target user: [description]
Business goal: [what the business needs]
Known constraints: [time / tech / brand / budget]

Output: 1) A clear problem statement, 2) 3 research questions to validate, 3) Draft success metrics, 4) Risks to watch.
```

---

## Phase 1 — Discovery & Research

See `research.md` for the full workflow.

### Key Inputs to Gather
- User interviews (5–8 for qualitative)
- Competitive audit (3–5 direct competitors)
- Stakeholder interviews (goals, constraints, politics)
- Existing analytics or usage data (if available)

### AI Assist — Competitive Audit Accelerator
```
Analyze [competitor name] as a UX/product strategist would.
Identify: 1) Core user flows, 2) UX strengths, 3) Friction points, 4) Positioning gaps.
Compare against: [your product or concept].
Output as a comparison table.
```

---

## Phase 2 — Define & Synthesize

**Goal:** Turn research data into clear, prioritized design direction.

### Deliverables
- Refined personas (2–3 max)
- Journey map (current state)
- Insight statements ("We discovered that...")
- HMW questions ("How might we...")
- Design principles for this project

### AI Assist — Persona Refinement
```
Based on these research notes: [paste notes]
Generate a UX persona with:
- Name, role, age, context
- Top 3 goals
- Top 3 pain points
- Key behaviors
- A representative quote
- What success looks like for them
Keep it grounded in the data — flag anything assumed.
```

### AI Assist — Insight to HMW
```
Convert these raw research insights into "How Might We" questions:
[paste insights]
Format: One HMW per insight. Prioritize by user impact.
```

---

## Phase 3 — Ideation & Concept Design

**Goal:** Generate multiple solution directions before committing to one.

### Methods
- Crazy 8s (sketching) → Stitch or Figma Make for rapid digitization
- Feature prioritization matrix (impact vs. effort)
- Design principles filter (does this concept honor our principles?)
- AI feature check: if the concept uses AI, run the **Designing for Trust checklist** below before prototyping

### AI Assist — Concept Generator
```
I'm designing [product/feature] for [persona].
Their biggest pain point is: [pain point]
Generate 3 distinct design concepts. For each:
- Core idea (1 sentence)
- Key interaction pattern
- Trade-off vs. the other concepts
- Best used when: [context]
```

### AI Assist — Feature Prioritization
```
Here is our feature list for [product]: [paste list]
Score each feature on:
- User impact (1–5)
- Business value (1–5)
- Implementation effort (1–5, where 5 = hardest)
Output as a prioritization table. Flag the top 5 for MVP.
```

---

## Phase 4 — Prototyping

**Goal:** Build the minimum fidelity needed to test your most critical assumption.

### Fidelity Decision Guide
| Test Goal | Right Fidelity | Right Tool |
|---|---|---|
| Validate concept direction | Low-fi wireframe | Figma (manual) or Stitch |
| Test user flow logic | Mid-fi clickable | Stitch or Figma Make |
| Test visual/brand direction | High-fi mockup | Figma |
| Stakeholder sign-off | Polished prototype | Figma + Stitch |
| Investor/client demo | Presentation-quality | Figma + Gamma |

### AI Assist — Stitch Prompt (User Flow)
```
Create a [screen type] screen for [product name].
User goal: [what they are trying to do]
Key elements: [list UI elements needed]
Tone/brand: [describe visual direction]
Flow: This screen comes after [previous screen] and leads to [next screen].
```

### AI Assist — Figma Make Prompt (Component)
```
Generate a [component type, e.g. onboarding card] component.
Context: [product name, user segment]
Must include: [list requirements]
Style: [minimal / bold / friendly / professional]
Accessibility: Ensure sufficient contrast and touch targets.
```

---

## Phase 5 — User Testing

See `research.md` → Testing section for the full workflow.

### Quick Test Plan Structure
1. **Objective** — What assumption are we testing?
2. **Tasks** — 3–5 specific tasks for the participant
3. **Success criteria** — How will you know it worked?
4. **Metrics** — Task completion rate, time on task, error rate, satisfaction score
5. **Debrief prompt** — Open-ended question after each task

### AI Assist — Test Script Generator
```
Write a usability test script for [prototype name].
Testing platform: [Maze / Zoom / in-person]
Prototype covers: [describe flows]
Key assumptions to test: [list 2–3]
Output: Intro script, 4 task prompts, debrief questions.
Keep language neutral — avoid leading the participant.
```

---

## Phase 6 — Iteration & Handoff

**Goal:** Translate test findings into design decisions and prepare for development.

### Handoff Checklist
- [ ] All screens annotated with behavior notes
- [ ] Component library organized and named
- [ ] Interaction specs documented (hover, error, empty states)
- [ ] Edge cases covered
- [ ] Accessibility checked (contrast, labels, touch targets)
- [ ] Research readout delivered to stakeholders (see `research.md`)

### AI Assist — Annotation Generator
```
I have a [screen name] screen with these elements: [list elements]
Write design annotations for a developer handoff. For each element include:
- Behavior description
- States (default, hover, active, error, disabled)
- Any conditional logic
Keep technical language appropriate for a front-end developer.
```

---

---

## Designing for Trust with AI — Ethics Checklist

Run this whenever a product feature uses AI to generate recommendations, automate decisions, or process user data. Increasingly a client expectation, not a nice-to-have.

### Transparency
- [ ] Does the UI clearly communicate when AI is making a recommendation (vs. a human or rule-based system)?
- [ ] Is there a plain-language explanation of *why* the AI made that recommendation?
- [ ] Are users told what data is being used to personalize their experience?

### User Control
- [ ] Can users override, dismiss, or customize AI recommendations?
- [ ] Can users opt out of AI-driven personalization?
- [ ] Is there a feedback mechanism ("Was this helpful?" / "Not for me")?

### Error & Failure States
- [ ] Is there a graceful fallback if the AI returns a poor or empty result?
- [ ] Are AI errors framed helpfully — not as system failures, but as "here's what to do next"?
- [ ] Does the design avoid the "black box" effect — where users can't tell why something happened?

### Bias & Fairness
- [ ] Has the AI feature been reviewed for outputs that could be discriminatory or exclusionary?
- [ ] Does the design avoid reinforcing stereotypes through AI-generated content or imagery?
- [ ] Are edge cases for non-mainstream users explicitly designed for?

### Data & Privacy
- [ ] Is data collection clearly disclosed at the point of collection?
- [ ] Is the minimum necessary data being collected?
- [ ] Are users able to delete their data or reset their AI profile?

### AI Assist — Trust Review Prompt
```
Review this AI-powered feature for trust and transparency issues: [describe feature]
Product: [name], User: [persona]
Check against:
1. Is the AI's role clear to the user?
2. Can users understand and control what the AI does?
3. Are failure states and edge cases handled gracefully?
4. Are there potential bias or fairness risks?
5. Is data use transparent and minimal?
Output: A prioritized list of trust gaps with specific design fixes for each.
```

---

## AI Integration Principles (Apply Throughout)

1. **AI starts, humans decide.** Use AI for first drafts, synthesis, and options — not final decisions.
2. **Context in, quality out.** The more specific your prompt context, the better the output. Never prompt without user/business context.
3. **Iterate fast.** Run 2–3 prompt variations on anything important. Pick the best, refine from there.
4. **Validate with real users.** AI-generated designs and copy must be tested. Never ship without user validation.
5. **Design for trust.** Any AI-powered feature must pass the ethics checklist above before moving to prototype.
6. **Document your prompts.** If a prompt works well, save it to `prompts.md`.
