---
description: "Start here — set up your AI workspace or get coaching to improve it"
argument-hint: ""
---

# /alusta — Your AI Starting Point

This command adapts to where you are:

## How It Works

**First, detect workspace state:**

1. Check if `CLAUDE.md` exists in the project root
2. Check if `.auto-memory/MEMORY.md` exists
3. Check which Kasulik plugins are installed

**Then route to the right mode:**

### 🆕 No CLAUDE.md found → First-Time Setup
"Welcome! Let's set up your AI workspace so I can help you effectively."
→ Load and follow the **workspace-setup** skill
→ Quick setup (5-10 min) first, offer deep mode after

### 🔧 CLAUDE.md exists but basic → Improvement Mode  
"Your workspace is set up. Let's make it more powerful."

Offer choices:
1. **Deepen your context** — update CLAUDE.md with more business detail
2. **Create a custom skill** — build workflows specific to your business
3. **Learn workflow recipes** — discover multi-skill workflows for your daily tasks
4. **Get coaching** — tips on prompting and iteration

### 🚀 CLAUDE.md + memory mature → Coaching Mode
"You're up and running! What can I help you improve?"
→ Load and follow the **ai-coach** skill
→ Offer: run `/review` for weekly check-in, `/workflows` for recipe reference

## What I Need From You

Just run `/alusta` — I'll figure out where you are and guide you from there.

If this is your first time: have your **company website URL** ready (if you have one). I'll research it so you don't have to explain everything from scratch.
