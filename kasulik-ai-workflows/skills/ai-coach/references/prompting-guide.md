# Prompting Guide

Practical tips for getting better results from AI. Use this when coaching users who are struggling with output quality.

## The 4 Common Mistakes (and Fixes)

### Mistake 1: Too Vague
**Problem:** "Write me an email" with no context.
**Fix:** Add WHO, WHAT, WHY, and TONE.

| Before | After |
|--------|-------|
| "Write me an email" | "Write a follow-up email to a CFO who attended our demo yesterday. She was interested in the reporting features but concerned about implementation time. Tone: professional, reassuring, concise." |

**Coaching prompt:** "Who is this for, and what do you want them to do after reading it?"

### Mistake 2: Not Iterating
**Problem:** Accepting the first output without pushback.
**Fix:** Treat AI output as a first draft. Always push back at least once.

**Iteration starters:**
- "Make the headline more specific — include a number or timeframe"
- "This is too formal for our audience. Make it more conversational"
- "The structure is good but the opening is weak. Rewrite just the first paragraph"
- "Cut this by 40% — remove everything that isn't essential"
- "Add a specific example for the second point"

**Coaching prompt:** "What would you change if a junior team member wrote this?"

### Mistake 3: Wrong Tool for the Job
**Problem:** Using AI for tasks where it's not the best fit, or not using AI for tasks where it excels.

**AI excels at:**
- First drafts of any structured content (emails, proposals, SOPs)
- Research and summarization
- Brainstorming and ideation (generating options)
- Structured analysis (CRO, SEO, competitive)
- Repetitive writing with variations (email sequences, ad copy)
- Transforming content between formats (notes → email, transcript → summary)

**AI struggles with:**
- Decisions requiring current, real-time data (unless tools connected)
- Highly subjective creative vision (it can help, not lead)
- Tasks requiring your specific institutional knowledge (give it context first)
- Final sign-off (always review before sending)

**Coaching prompt:** "What would you spend your time on if AI handled the first draft?"

### Mistake 4: No Strategic Confidence
**Problem:** "Can AI really do this?" or treating AI as a toy, not a tool.
**Fix:** Start with a small, low-stakes win. Build from there.

**Confidence builders:**
1. Pick ONE recurring task that takes >30 min
2. Try it with AI — spend 10 min on context and iteration
3. Compare the result. Usually 80% as good in 20% of the time.
4. The 20% gap? That's where your expertise adds value on top.

**Coaching prompt:** "What's one task this week you wish you could delegate? Let's try it right now."

---

## The Context Sandwich

Best structure for any AI request:

```
CONTEXT: Who you are, what the business does, who this is for
TASK: What you need, in specific terms
CONSTRAINTS: Format, length, tone, what to avoid
EXAMPLE: (optional) A reference of what good looks like
```

**Example:**
```
CONTEXT: I run a B2B SaaS for project management. Our customers are 
mid-size agencies (20-100 people). Tone is professional but friendly.

TASK: Write a case study intro paragraph about a client (MarketForce, 
a 45-person marketing agency) who reduced project overruns by 60% 
after using our tool for 3 months.

CONSTRAINTS: 3-4 sentences. Lead with the result, not the company name. 
Don't use the word "streamline."
```

---

## Iteration Patterns

### The Refine Loop
1. Generate initial output
2. Identify the weakest part
3. Ask to improve JUST that part
4. Repeat until satisfied

### The Parallel Options
1. "Give me 3 different approaches to this headline"
2. Pick the best elements from each
3. "Combine the directness of option 1 with the specificity of option 3"

### The Role Shift
1. Get initial output
2. "Now review this as if you were a skeptical customer who's seen 100 landing pages"
3. Apply the critique to improve

### The Constraint Tightening
1. Get initial output (too long, too generic)
2. "Cut this to half the length, keeping only the most compelling points"
3. "Now make every sentence specific — replace any vague claim with a concrete detail"

---

## When Output Quality Drops

Diagnose the issue:

| Symptom | Likely Cause | Fix |
|---------|-------------|-----|
| Generic, could apply to anyone | No business context | Run /alusta or add context to CLAUDE.md |
| Wrong tone | No tone guidance | Specify tone explicitly or set up brand-voice-enforcement |
| Missing key points | Forgot to mention constraints | Use the Context Sandwich structure |
| Too long/verbose | No length constraint | Specify word count or "keep it under 3 paragraphs" |
| Factually wrong | AI hallucination | Ask it to cite sources or verify claims |
| Boring/flat | Accepted first draft | Iterate — "make this more [specific/bold/concrete]" |
