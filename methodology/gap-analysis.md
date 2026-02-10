# Gap Analysis Methodology

A framework for evaluating whether your writing voice prevents common AI patterns.

## Overview

The gap analysis methodology helps you assess how well your existing writing guidelines protect against AI writing patterns. Rather than building pattern detection from scratch, this approach:

1. Takes your existing voice guide (if you have one)
2. Evaluates it against known AI pattern lists
3. Identifies which patterns you already prevent vs. which need explicit coverage
4. Integrates missing patterns into your guidance

## The Core Insight

**Strong foundational writing principles prevent most AI patterns naturally.**

If your writing voice emphasizes clarity, precision, and authenticity, you're already preventing the majority of AI patterns without explicit rules. The gap analysis helps you find the edge cases that slip through.

## Step 1: Gather Your Materials

**You need:**
- Your writing voice guide (or style guidelines)
- A comprehensive list of AI writing patterns (we use the 24 from Wikipedia's "Signs of AI Writing")
- Examples of content in your voice

**If you don't have a voice guide yet:**
Start by documenting your natural writing principles. What do you avoid? What do you prefer? What feels authentic vs. performed?

## Step 2: Create the Evaluation Matrix

Build a simple table:

| Pattern | Already Prevented? | How? | Gap? |
|---------|-------------------|------|------|
| Surface-level -ing verbs | ? | ? | ? |
| Weak verb substitutions | ? | ? | ? |
| ... | | | |

## Step 3: Test Against Principles

For each AI pattern, ask:

1. **Does my voice guide explicitly address this?**
   - Example: "Avoid hedging language" directly prevents Pattern #20 (Excessive hedging)

2. **Does my voice guide implicitly prevent this?**
   - Example: "Use precise verbs" prevents weak verb substitutions even without naming them

3. **Could this pattern appear despite my guidelines?**
   - Example: Your guide might emphasize clarity but not explicitly flag formulaic triplets

## Step 4: Categorize Results

**Category A: Already Prevented**
- Your existing principles handle this
- No additional guidance needed
- Document the connection for reference

**Category B: Partially Prevented**
- Your principles lean toward prevention but edge cases exist
- Consider explicit examples to reinforce

**Category C: Gap Identified**
- This pattern could slip through
- Needs explicit coverage

## Step 5: Integrate Gaps

For Category C patterns:

**Option 1: Expand Existing Principles**
Add the pattern as an example under relevant existing guidance.

Example: Your guide says "avoid filler" → add "including formulaic triplets like 'innovation, inspiration, and implementation'"

**Option 2: Create New Section**
If multiple gaps cluster around a theme, create a dedicated section.

Example: "AI Pattern Edge Cases" or "Mechanical Phrases to Avoid"

**Option 3: Use Detection Tool**
For patterns that are hard to prevent through general principles, use automated detection.

Example: False scope ranges ("from X to Y") benefit from tooling

## Step 6: Validate

Test your updated guidelines:

1. Take content you've written
2. Check for the gap patterns
3. Revise guidance if needed
4. Repeat with fresh examples

## Real-World Example

**Voice Principle:** "No filler, no padding. Every sentence does work."

**Patterns Prevented:**
- ✅ Unnecessary qualifiers (Pattern #18)
- ✅ Excessive hedging (Pattern #20)
- ✅ Filler phrases (Pattern #21)
- ✅ Generic transitions (Pattern #22)
- ✅ Vapid closings (Pattern #24)

**Patterns NOT Prevented:**
- ⚠️ Formulaic triplets (Pattern #11) — not obviously "filler"
- ⚠️ False scope ranges (Pattern #17) — can sound substantive

**Solution:** Add explicit examples under the "no filler" principle.

## When to Use Tooling vs. Guidelines

**Use guidelines for:**
- Patterns that violate clear principles (hype language, hedging)
- Patterns you can teach yourself to avoid (weak verbs)
- Patterns that affect overall voice (mechanical transitions)

**Use detection tools for:**
- Subtle patterns that are hard to self-catch (surface-level -ing verbs)
- Patterns that require comparison (scope ranges, data dumps)
- High-frequency checks when editing others' work

## Maintenance

Voice guides evolve. Revisit your gap analysis:

- When new AI patterns emerge
- When your writing voice shifts
- When you notice new patterns in your work
- Annually as a calibration check

## Common Pitfalls

**Pitfall 1: Assuming coverage without testing**
Don't guess. Actually check your content against the patterns.

**Pitfall 2: Over-indexing on pattern lists**
Your authentic voice matters more than perfect pattern avoidance.

**Pitfall 3: Adding rules without understanding why**
Each guideline should serve your voice, not just check a box.

**Pitfall 4: Forgetting the principle**
Pattern lists change. Strong foundational principles are portable.

## Results to Expect

A typical gap analysis finds:

- 60-80% of patterns already prevented by good writing principles
- 10-20% partially prevented (need minor reinforcement)
- 10-20% true gaps requiring explicit coverage

If you're preventing fewer than 50% naturally, your voice guide may need foundational strengthening before pattern-specific work.

## Next Steps

1. Download the [24 AI patterns reference](../humanizer-skill/patterns.md)
2. Create your evaluation matrix
3. Test systematically
4. Integrate gaps into your voice guide
5. Use the [humanizer skill](../humanizer-skill/) for automated detection

## Resources

- [Wikipedia: Signs of AI Writing](https://en.wikipedia.org/wiki/Artificial_intelligence_detection#Signs_of_AI_writing)
- [Humanizer skill pattern reference](../humanizer-skill/patterns.md)
- [Integration guide for Claude skills](../docs/integration.md)
