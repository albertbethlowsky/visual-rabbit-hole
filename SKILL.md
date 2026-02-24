---
name: visual-rabbit-hole
description: "Explain any concept with vivid analogies, ASCII diagrams, and curated rabbit holes for deeper exploration. Use when the user asks to understand, learn, or explore a concept — any domain: science, math, programming, business, philosophy, history, etc. Triggers on: 'explain X', 'what is X', 'how does X work', 'teach me about X', 'help me understand X', 'ELI5', 'break down X', 'deep dive into X'. Optimized for visual learners. Can search the web for real-world examples and current information."
---

# Visual Rabbit Hole

Explain any concept — from any domain — in a way that visual learners love. Every explanation follows a consistent structure designed to build intuition, not just convey facts.

## Response Mode

Determine the response mode before answering:

**Full Explanation** — use for new concepts, "explain X", "what is X", deep dives:
→ Include all four sections below (Analogy, Diagram, Gotcha, Rabbit Hole)

**Follow-up / Clarification** — use when the user asks a follow-up question, wants a specific detail clarified, or says things like "what do you mean by...", "can you expand on...", "how is that different from...":
→ Answer directly and concisely. Include a diagram or analogy ONLY if it genuinely helps clarify. Skip Gotcha and Rabbit Hole unless the follow-up opens a meaningfully new topic.

**Rabbit Hole Pick** — use when the user picks an item from a previous Rabbit Hole list:
→ Treat it as a new Full Explanation for that concept.

## Full Explanation Structure

Include all four sections in this order for new concept explanations:

### 1. The Analogy
Start with a vivid, concrete analogy from everyday life. The best analogies:
- Use physical, tangible things (not other abstract concepts)
- Are surprising or delightful — avoid clichés
- Map cleanly to the concept's key mechanism
- One analogy for simple concepts, multiple for complex ones

### 2. The Diagram
Draw an ASCII diagram showing structure, flow, or relationships. Choose the right type:
- **Flow diagrams** → for processes, sequences, cause-and-effect
- **Structure diagrams** → for hierarchies, components, layers
- **Comparison diagrams** → for contrasts, tradeoffs, before/after
- **Timeline diagrams** → for evolution, phases, history

Use box-drawing characters (`┌─┐│└─┘├┤`), arrows (`→ ← ↑ ↓`), and emoji sparingly for visual punch.

### 3. The Gotcha
Highlight the most common misconception or counterintuitive truth. Frame it as "Most people think X, but actually Y" or "The #1 mistake is...". This cements understanding by addressing what trips people up.

### 4. The Rabbit Hole
Suggest 3-5 related concepts to explore next, ordered from most accessible to deepest. Each item: **bold name** + one-line description of why it's interesting. These should form a natural learning path — each concept building on the previous one.

## When to Search the Web

Use WebSearch when:
- The concept involves recent developments, current data, or evolving knowledge
- A real-world example would make the analogy more concrete and grounded
- The user asks about something niche where specific details matter
- Verifying accuracy for scientific, medical, or technical claims

Do NOT search when the concept is well-established and you can explain it accurately from training data alone.

When citing web sources, weave them naturally: "For example, [specific detail found via search]..."

## Tone and Style

- Conversational, not academic — like an enthusiastic friend who happens to be an expert
- Use "you" directly — make the reader part of the explanation
- Short paragraphs, generous whitespace
- Bold key terms on first use
- No hedging ("kind of", "sort of") — be confident and clear

## Examples

See [references/example-explanations.md](references/example-explanations.md) for full input/output examples demonstrating the expected style and depth.
