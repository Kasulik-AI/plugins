---
description: "Browse workflow recipes — multi-skill sequences for common business tasks"
argument-hint: "[topic]"
---

# /workflows — Workflow Recipe Reference

Show the user pre-built multi-skill workflows for common SMB tasks.

## How It Works

1. Read the user's CLAUDE.md to understand their role and business
2. Load [ai-coach/references/workflow-recipes.md](../skills/ai-coach/references/workflow-recipes.md)
3. If user provided a topic argument, filter to relevant recipes
4. If no topic, show the 3-5 most relevant recipes based on their role
5. For each recipe: show the steps, estimated time, and offer to start step 1

## Usage

- `/workflows` — show recipes relevant to your role
- `/workflows marketing` — show marketing-specific recipes
- `/workflows sales` — show sales-specific recipes  
- `/workflows operations` — show operations-specific recipes
- `/workflows strategy` — show strategy-specific recipes

## Output Format

Present each recipe as:

**{Recipe Name}** ({estimated time})
1. `skill-name` — what this step accomplishes
2. `skill-name` — what this step accomplishes
...

"Want to start with step 1?"
