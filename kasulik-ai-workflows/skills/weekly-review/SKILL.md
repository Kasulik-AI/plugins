---
name: weekly-review
description: "Weekly AI workspace review — reflects on what worked, updates memory, suggests improvements, and identifies underused skills. Triggers on: 'weekly review', 'review my week', 'check in', 'how am I doing with AI', 'weekly reflection', 'improve my AI usage', or when scheduled as a recurring task."
---

# Weekly Review

A structured 15-minute reflection that improves the user's AI workspace over time.

## Before Starting

1. Read CLAUDE.md for business context and current setup
2. Read MEMORY.md and recent memory files for what's been learned
3. Check which Kasulik plugins are installed

## Review Flow

### Step 1: Wins (2 min)

Ask: "What went well this week with AI? Any tasks where it saved you real time or produced great output?"

Listen for:
- Specific skills that worked well → reinforce these in memory
- Workflows that clicked → note the pattern
- Confidence growth → acknowledge it

Save wins to memory if they contain reusable insights.

### Step 2: Struggles (3 min)

Ask: "Where did AI fall short this week? Any frustrations or tasks where the output wasn't useful?"

Diagnose:
- Was it a prompting issue? → Teach the fix (reference prompting-guide.md via ai-coach)
- Was it the wrong skill? → Recommend a better one
- Was it missing context? → Suggest updating CLAUDE.md
- Was it an actual AI limitation? → Acknowledge honestly and suggest alternatives

### Step 3: Discovery (3 min)

Based on their role and what they've been doing, suggest 1-2 skills they haven't tried:

"Based on your work this week, you might find these useful:
- **[skill name]**: [one sentence on why it fits their situation]
- Want me to show you how it works with a quick example?"

Only suggest skills from plugins they have installed.

### Step 4: Workspace Health (3 min)

Check and suggest improvements:

- **CLAUDE.md**: Is it still accurate? Any new context to add?
- **Memory**: Any new learnings worth persisting? Any stale memories to update?
- **Workflows**: Are there recurring tasks that should become a workflow recipe?
- **Custom skill**: If they don't have one, is it time to create one?

### Step 5: Next Week (2 min)

Ask: "What's your biggest priority next week? Let me suggest how AI can help."

Map their answer to specific skills and propose a mini-plan.

### Step 6: Update

Based on the conversation:
1. Update any relevant memory files
2. Suggest CLAUDE.md edits if needed (show diff, let user approve)
3. Save any new workflow patterns discovered

## Output Format

End with a brief summary:

```
## Weekly Review — {date}

**Wins**: {1-2 bullet summary}
**Improved**: {what was fixed or learned}
**Try next week**: {1-2 skill suggestions with why}
**Workspace updates**: {what was changed in CLAUDE.md or memory}
```

## Scheduling

This review can be set up as a scheduled task. Suggest:
"Want me to schedule this as a weekly check-in? I can set it up to run every Friday at the end of your work day."

If the scheduled-tasks MCP is available, use it to create the recurring task.

## Key Principles

- **Celebrate before critiquing** — always start with wins
- **One improvement at a time** — don't overwhelm with 5 suggestions
- **Concrete over abstract** — "Try draft-outreach for your Acme lead" not "explore more skills"
- **User drives the pace** — some weeks are light, that's fine
- **Build the habit** — consistency matters more than depth
