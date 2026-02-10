---
name: humanizer
description: Detects and flags AI writing patterns in text. Use when reviewing content for authenticity, editing AI-generated text, or checking your own writing for mechanical patterns. Identifies 24 documented patterns across categories including content structure, language choices, style markers, communication patterns, and filler language. Returns specific pattern violations with examples and suggestions.
---

# Humanizer Skill

Detects AI writing patterns based on Wikipedia's "Signs of AI Writing" maintained by WikiProject AI Cleanup.

## When to Use This Skill

- Reviewing content for AI writing patterns
- Editing text to sound more natural and authentic
- Quality-checking your own writing when working with AI tools
- Training yourself to recognize and avoid these patterns

## How It Works

Analyzes text against 24 documented AI writing patterns organized in five categories:

1. **Content & Structure** — How information is organized and presented
2. **Language Choices** — Word selection and verb usage
3. **Style Markers** — Sentence construction and rhythm
4. **Communication Patterns** — How ideas are expressed and connected
5. **Filler & Hedging** — Unnecessary qualifiers and weak closings

## The 24 Patterns

### Content & Structure

**1. Unnecessarily long paragraphs**
Dense blocks of text without natural breaks. AI tends to pack information rather than letting ideas breathe.

**2. Data dumps**
Listing facts or statistics without context or narrative. Example: "In 2019, sales were $5M. In 2020, $6.2M. In 2021, $7.8M." vs. "Sales grew 24% annually from 2019-2021."

**3. Outdated information**
References to events, data, or trends that are no longer current. Check dates and claims.

**4. Surface-level -ing verbs (participial phrases)**
Using descriptive -ing phrases instead of direct action. Example: "The platform, symbolizing innovation and reflecting modern needs..." vs. "The platform enables real-time collaboration."

### Language Choices

**5. Weak verb substitutions**
Using phrases like "serves as" or "acts as" instead of direct verbs. Example: "The tool serves as a solution" vs. "The tool solves" or "The tool is a solution."

**6. Passive voice overuse**
"The decision was made" vs. "We decided." Passive voice distances the writing from action.

**7. Noun clusters**
Stacking nouns together. Example: "customer relationship management system optimization" vs. "optimizing how we manage customer relationships."

**8. Redundancies**
Saying the same thing twice. Example: "past history," "end result," "future plans," "collaborate together."

**9. Unnatural phrasings**
Constructions that sound AI-generated. Example: "It's worth noting that..." (just state the thing), "One might consider..." (who is "one"?).

**10. Misused jargon**
Using technical terms incorrectly or where simpler language would be clearer.

### Style Markers

**11. Formulaic triplets (rule of three)**
Always grouping things in threes. Example: "Innovation, inspiration, and implementation" when the natural count might be two or four items.

**12. Title case overuse**
Capitalizing common concepts unnecessarily. Example: "Our Strategy for Growth" vs. "our strategy for growth."

**13. Robotic transitions**
Mechanical connectors between ideas. Example: "Furthermore," "Moreover," "In addition," used repetitively. Natural writing varies transitions or implies connections.

**14. Clichéd metaphors**
Overused comparisons. Example: "tip of the iceberg," "paradigm shift," "game changer," "low-hanging fruit."

**15. Uniform sentence structure**
Every sentence following the same pattern. Lack of rhythm variation.

**16. Comma splices**
Connecting independent clauses with just a comma. Example: "The project was delayed, the team worked overtime." Needs: semicolon, period, or conjunction.

**17. False scope ranges**
Claiming to cover more ground than actually addressed. Example: "From basic setup to enterprise architecture" when only covering mid-level features.

### Communication Patterns

**18. Unnecessary qualifiers**
Weakening statements with excessive modifiers. Example: "somewhat," "quite," "rather," "fairly," "relatively," "arguably."

**19. Listiness**
Over-reliance on bullet points and numbered lists when prose would be more natural. Every response formatted as a list.

**20. Excessive hedging**
Too many disclaimers. Example: "It might be possible that one could perhaps consider..." Just state your point.

**21. Filler phrases**
Empty language that adds no meaning. Examples:
- "It's important to note that..."
- "It should be emphasized that..."
- "As a matter of fact..."
- "At the end of the day..."
- "When it comes to..."

**22. Generic transitions**
Cookie-cutter phrases connecting ideas. Example: "In today's fast-paced world," "In an increasingly digital landscape," "As we move forward."

**23. Overuse of Latin/Greek affixes**
Adding -ize, -ification, -ation unnecessarily. Example: "utilization" vs. "use," "optimization" vs. "improving."

### Filler & Hedging

**24. Vapid closings**
Generic endings with no substance. Examples:
- "The future looks bright for..."
- "Only time will tell..."
- "It remains to be seen..."
- "The possibilities are endless..."

Instead: End with a specific next step, concrete data point, or thought-provoking observation.

## Usage Instructions

**To check text:**
Simply paste the content and ask: "Check this for AI writing patterns."

**Example request:**
> Check this draft for AI writing patterns:
> 
> [your text here]

**What you'll get back:**
- Patterns identified with specific examples from your text
- Category labels (Content, Language, Style, Communication, Filler)
- Suggestions for revision
- Overall assessment

## How to Interpret Results

**High pattern count (10+ violations):**
Text likely needs significant revision. Consider rewriting from scratch with your authentic voice rather than editing incrementally.

**Medium pattern count (4-9 violations):**
Specific issues to address. Edit for the flagged patterns, then check again.

**Low pattern count (1-3 violations):**
Minor cleanup needed. Good overall authenticity.

**No patterns detected:**
Either excellent natural writing or the patterns are more subtle. Consider having a human reader check for voice authenticity.

## Limitations

This skill detects **patterns**, not quality. Some legitimate writing might trigger flags (academic papers sometimes need passive voice, technical documentation sometimes needs noun clusters).

Use judgment. The goal is authentic voice, not pattern avoidance for its own sake.

## Integration with Voice Guides

This skill works best alongside your own writing principles:

1. **Start with your voice guide** — What's your natural style?
2. **Use this skill for edge case detection** — Catch what your principles miss
3. **Refine iteratively** — Learn which patterns you personally struggle with

See the [integration guide](../docs/integration.md) for details on combining this skill with your writing voice.

## Philosophy

From Wikipedia's AI Writing guide:

> "Avoiding AI patterns is only half the job. Sterile, voiceless writing is just as obvious as slop."

The goal isn't to eliminate all patterns mechanically. It's to write with authentic voice. These patterns are signals, not rules.

## Credits

Pattern list sourced from Wikipedia's "Signs of AI Writing" article, maintained by WikiProject AI Cleanup.

Skill implementation inspired by Siqi Chen's [humanizer skill](https://github.com/blader/humanizer).

## Version

1.0.0 — February 2026
