# PITCH.md
## Business Case, Value Proposition & Pitch Frameworks

For translating design work into business language and building compelling stakeholder narratives. Covers the Value Proposition Canvas, pitch deck structure, ROI measurement, and AI-assisted content generation using Gamma.app.

---

## 1. Value Proposition Canvas

Use this to ensure product design is solving real customer problems — and to build the foundation of any pitch.

### Customer Profile
**Step 1 — Customer Jobs** *(what they're trying to achieve)*
AI Prompt:
```
Generate a list of functional, social, and emotional jobs for [target user] trying to [achieve goal].
Functional jobs = practical tasks they need to complete
Social jobs = how they want to be perceived
Emotional jobs = how they want to feel
Product context: [describe product]
```

**Step 2 — Customer Pains** *(frustrations, blockers, risks)*
AI Prompt:
```
What are the biggest pains experienced by [target user] when trying to [achieve goal]?
Categorize as: Undesired outcomes / Obstacles / Risks
Rank by severity (high / medium / low).
Be specific — avoid generic answers like "it's confusing."
```

**Step 3 — Customer Gains** *(desired outcomes and benefits)*
AI Prompt:
```
What gains does [target user] want when [achieving goal]?
Categorize as: Required gains / Expected gains / Desired gains / Unexpected gains
Focus on measurable or observable outcomes where possible.
```

### Value Map
**Step 4 — Products & Services** — List your core features/capabilities

**Step 5 — Pain Relievers**
AI Prompt:
```
For each of these customer pains: [paste pains]
Describe how [product name] relieves that pain.
Be specific — connect each pain directly to a feature or design decision.
Flag any pain we currently don't address.
```

**Step 6 — Gain Creators**
AI Prompt:
```
For each of these customer gains: [paste gains]
Describe how [product name] creates that gain.
Rate our strength on each gain: Strong fit / Partial fit / Gap
Suggest one product enhancement for each gap.
```

### Fit Assessment
```
Review this completed Value Proposition Canvas: [paste canvas summary]
Assess the fit:
1. Which pains are we relieving most strongly? (evidence-based)
2. Which gains are we creating most effectively?
3. Where is the fit weakest?
4. What's the single most compelling value proposition statement we should lead with?
Write a one-sentence value proposition: "[Product] helps [target user] [achieve job] by [key mechanism] so they can [ultimate gain]."
```

---

## 2. Pitch Deck Structure

Standard structure for a product/design pitch. Adapt based on audience (internal stakeholder vs. client vs. investor).

### Slide Framework
| Slide | Purpose | Key Content |
|---|---|---|
| 1. Hook | Grab attention | Provocative stat, problem statement, or user quote |
| 2. Problem | Define the pain | Specific, relatable, evidence-backed |
| 3. User | Make it human | Persona or real user story |
| 4. Market Opportunity | Show the size | Market data, trend, underserved segment |
| 5. Solution | Your answer | Product demo, key screens, core value prop |
| 6. How It Works | Explain the mechanism | Flow diagram, key interaction |
| 7. Evidence | Prove it works | Research findings, test results, metrics |
| 8. Business Model | Show the money | Revenue model, pricing, unit economics |
| 9. Roadmap | Show momentum | MVP → V1 → V2 milestones |
| 10. Team / Ask | Close the loop | Credentials + what you need from this audience |

### AI Assist — Pitch Narrative Generator (Gamma.app or Claude)
```
Help me write a pitch narrative for [product name].
Audience: [investors / internal stakeholders / client / board]
Product: [description]
Target user: [description]
Key problem: [description]
Our solution: [description]
Evidence we have: [research findings, test results, metrics]
Ask: [funding / approval / resources / sign-off]

Write a 10-slide narrative arc. For each slide: slide title, 3-bullet content, and one data point or quote to include.
Tone: [confident / visionary / pragmatic — pick one]
```

### AI Assist — Hook Slide Generator
```
Write 3 opening hook options for a pitch about [product/problem].
Audience: [description]
Each hook should be: unexpected, specific, and make the audience feel the problem.
Format options:
A) A surprising statistic
B) A user story (30 seconds to read aloud)
C) A provocative question
```

---

## 3. ROI & Business Case for Design

Use when you need to justify design investment to a business stakeholder.

### Design ROI Framework
Map design decisions to business metrics:

| Design Decision | User Outcome | Business Metric |
|---|---|---|
| Simplified onboarding | Users complete setup faster | Activation rate ↑ |
| Clearer CTA copy | More users take desired action | Conversion rate ↑ |
| Reduced error states | Fewer support contacts | Support cost ↓ |
| Improved navigation | Users find features faster | Feature adoption ↑ |
| Accessibility improvements | More users served | TAM expansion |

### AI Assist — ROI Case Builder
```
I made this design change: [describe change]
Here is the before/after data: [paste metrics if available]
Target audience for this business case: [VP Product / CFO / client / board]

Build a business case:
1. Problem cost (what the old design was costing — in users, revenue, or time)
2. Solution impact (what the new design delivers — be conservative)
3. Investment required (design time, dev time)
4. Projected ROI (timeline to value)
5. Risk of not acting
Format for a 2-minute verbal pitch + 1 supporting slide.
```

### Key Metrics by Project Type
| Project Type | Metrics to Track |
|---|---|
| Onboarding redesign | Activation rate, time-to-value, drop-off by step |
| Feature redesign | Feature adoption, task completion rate, support ticket volume |
| Navigation overhaul | Time on task, search usage rate, feature discoverability |
| New product | Retention (Day 1, 7, 30), NPS, conversion rate |
| Research-informed redesign | Qualitative: theme resolution rate / Quantitative: chosen above |

---

## 4. Building Decks in Gamma.app

### Gamma Workflow for Fast Pitch Decks
1. Start with the Claude pitch narrative prompt above — get your 10-slide outline first
2. Open Gamma → "Generate presentation"
3. Paste your narrative outline into Gamma's AI input
4. Choose a visual theme that matches the product's brand tone
5. Review each slide: replace placeholder content with your actual data
6. Use Gamma's "Remix" feature to adjust tone or structure
7. Export as PDF for stakeholder delivery or present live via Gamma link

### Gamma Prompt Tips
- Give Gamma a clear narrative arc — it performs better with structured input than free-form descriptions
- Specify the audience in your prompt: "This is for a VP audience who values speed and business impact"
- If slides feel generic, add specific details: product name, actual metrics, real user quotes
- Use Gamma's image generation for conceptual visuals; replace with real screenshots for later-stage pitches

### AI Assist — Gamma Slide Content Polish
```
Here is a rough slide for my pitch: [paste slide content]
Audience: [description]
Rewrite it to be:
- Cleaner (fewer words, same meaning)
- More specific (replace vague claims with data or examples)
- More compelling (lead with the insight, not the context)
Output: Revised headline + 3 bullet points. Max 8 words per bullet.
```

---

## 5. Advocating for AI Tools Internally

Use when pitching AI tool adoption to a team or organization.

### The Advocacy Framework
1. **Start with a pain, not a tool** — "We spend X hours on Y task" beats "we should use AI"
2. **Show, don't tell** — Run a live demo with a real project example
3. **Quantify the gain** — Time saved, quality improved, bottleneck removed
4. **Address the fear** — Data privacy, job replacement, quality control
5. **Propose a pilot** — Low-risk, time-boxed, with clear success criteria

### AI Assist — Internal Advocacy Pitch
```
Help me write an internal pitch for adopting [AI tool] at [company/team level].
Current pain: [what takes too long or costs too much]
Tool solution: [what the tool does / how it solves the pain]
Audience concerns: [list likely objections: cost / privacy / learning curve / job security]
Pilot proposal: [what you want to test, for how long, with what success criteria]

Output:
1. One-paragraph executive summary
2. Objection-handling table (objection → response)
3. Pilot proposal outline
4. Success metrics for the pilot
```
