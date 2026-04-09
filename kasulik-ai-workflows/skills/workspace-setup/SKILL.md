---
name: workspace-setup
description: "Set up a new AI workspace from scratch or deepen an existing one. Triggers on: 'set up my workspace', 'new project', 'configure my Claude', 'I'm new here', 'set up project', 'blank project setup', or when no CLAUDE.md exists and user needs onboarding. Creates CLAUDE.md, memory files, and optionally a custom skill tailored to the user's business."
---

# Workspace Setup

Adaptive onboarding that turns a blank Claude workspace into a configured environment for a specific business or project.

## State Detection

Before starting, check what already exists:

1. Check for `CLAUDE.md` in the project root
2. Check for `.auto-memory/MEMORY.md` or `memory/` directory
3. Check which Kasulik plugins are installed (glob for `**/plugin.json` with "kasulik" in name)

**No CLAUDE.md** → Full setup (Quick mode first, offer Deep mode after)
**CLAUDE.md exists but basic** → Improvement mode (offer to enrich, add custom skill)
**CLAUDE.md + memory + custom skill** → Redirect to ai-coach skill

## Quick Setup Flow (5-10 minutes)

### Step 1: Core Interview

Ask ONE question at a time. Use multiple-choice when possible.

1. "What's your business/project name?"
2. "What does your business do? (one sentence)"
3. "Do you have a website I can research?" → If yes, use WebSearch/WebFetch to pull:
   - What the company does
   - Target audience signals
   - Product/service offerings
   - Tone and language patterns
4. "What's your role?" (founder, marketing lead, operations, sales, etc.)
5. "What will you primarily use AI for?" (multiple choice: marketing/content, sales/outreach, operations/processes, strategy/planning, all of the above)

### Step 2: Generate CLAUDE.md

Use the template in [references/claude-md-template.md](references/claude-md-template.md).

Write to `CLAUDE.md` in the project root. Include:
- Business context (name, what they do, audience)
- User's role and primary use cases
- Tone/voice guidance derived from website research
- Which Kasulik plugins are installed and their key skills
- Quick-reference: "For X, try Y skill"

### Step 3: Create Memory Files

Create `.auto-memory/` directory with:

**MEMORY.md** (index):
```markdown
- [Business context](user_business.md) — {company} overview, audience, positioning
- [User profile](user_profile.md) — {name}, {role}, primary AI use cases
```

**user_business.md**:
```markdown
---
name: Business context
description: {company} — {one-liner about what they do}
type: user
---
{Details from interview and website research}
```

**user_profile.md**:
```markdown
---
name: User profile
description: {name}, {role} at {company} — uses AI for {primary use cases}
type: user
---
{Role, experience level, goals}
```

### Step 4: Offer Deep Mode

After quick setup completes, ask:

"Your workspace is ready. Want me to go deeper? I can:
1. **Create a custom skill** for your specific workflows (10-15 min)
2. **Set up workflow recipes** for your daily tasks (5 min)
3. **That's enough for now** — you can always run /alusta again later"

## Deep Setup: Custom Skill Creation

If user chooses option 1:

1. Extended interview about their specific workflows:
   - "Walk me through a typical work week — what tasks repeat?"
   - "What content do you create most often?"
   - "What decisions do you make regularly that AI could help with?"
   - "Any specific terminology, templates, or processes unique to your business?"

2. Create a custom skill at `skills/{business-name}-workflows/SKILL.md`:
   - Business-specific terminology and context
   - Common task templates (email formats, report structures, etc.)
   - Decision frameworks specific to their industry
   - Links to their product-marketing-context if it exists

3. Name the skill `{business-name}-workflows` (e.g., `acme-workflows`)

## Deep Setup: Workflow Recipes

If user chooses option 2:

Read [references from ai-coach skill](../ai-coach/references/workflow-recipes.md) and present the 3-5 most relevant recipes based on user's role and primary use cases. Save selected recipes to memory.

## Key Principles

- **One question at a time** — never dump a form
- **Research before asking** — if they give a URL, extract what you can before asking more
- **Show progress** — use TodoWrite to show setup steps completing
- **Graceful defaults** — if user skips a question, use sensible defaults from research
- **Always end with a next step** — "Try asking me to [specific task relevant to their role]"
