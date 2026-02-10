# Integration Guide

How to adapt the humanizer skill for your own writing voice and workflow.

## Core Principle

**The humanizer skill is a detection tool, not a voice guide.**

Your writing voice should come from your own principles, preferences, and authentic style. The humanizer catches edge-case patterns that slip through even with strong foundational guidelines.

Think of it as: **Your voice guide does the heavy lifting. The humanizer catches what's left.**

---

## Integration Workflow

### Step 1: Define Your Writing Voice

Before integrating the humanizer, document your writing principles.

**Questions to answer:**
- What do you avoid? (hype language, hedging, jargon?)
- What do you prefer? (short sentences, contractions, direct language?)
- What feels authentic to you? (warm/clinical, casual/formal, expansive/economical?)
- What signals do you want to send? (expertise, care, efficiency, creativity?)

**Example voice principles:**
- "No filler, no padding. Every sentence does work."
- "Warm but functional. Not performative."
- "Respects the reader's intelligence. Information-dense."

Document these before looking at the pattern list.

---

### Step 2: Run a Gap Analysis

Use the [gap analysis methodology](../methodology/gap-analysis.md) to evaluate your voice guide against the 24 patterns.

**Create this matrix:**

| Pattern | Prevented by My Voice? | How? | Need Explicit Coverage? |
|---------|----------------------|------|------------------------|
| Unnecessarily long paragraphs | ✅ Yes | "Short sentences when making a point" | No |
| Weak verb substitutions | ✅ Yes | "Prefer precise verbs" | No |
| Formulaic triplets | ⚠️ Partial | Not explicitly covered | Yes |
| ... | | | |

**Expected results:**
- 60-80% naturally prevented by good writing principles
- 10-20% partially prevented (could use reinforcement)
- 10-20% true gaps (need explicit attention)

---

### Step 3: Decide What to Add to Your Voice Guide

For patterns in the "gap" category, choose:

**Option A: Expand Existing Principles**

Add the pattern as an example under relevant guidance.

Example:
```markdown
## Language

Avoid filler and unnecessary qualifiers.
- ❌ Hedging: "maybe," "perhaps," "possibly"
- ❌ Formulaic triplets: "innovation, inspiration, and implementation"
- ✅ Natural count: state what's actually there
```

**Option B: Create New Section**

If you have 5+ gap patterns, consider a dedicated section.

Example:
```markdown
## AI Pattern Edge Cases

Your core principles prevent most AI patterns. These five can slip through:

1. **Surface-level -ing verbs** — [explanation + examples]
2. **Weak verb substitutions** — [explanation + examples]
...
```

**Option C: Rely on Tool Detection**

For patterns that are hard to internalize, let the humanizer catch them during editing.

---

### Step 4: Customize the Humanizer Skill

Edit the SKILL.md file to align with your voice.

**What to customize:**

1. **Pattern priority**
   - Reorder patterns by what YOU struggle with most
   - Remove patterns you never violate
   - Add emphasis to your weak spots

2. **Examples**
   - Replace generic examples with ones from your domain
   - Use your actual writing as before/after cases
   - Make examples match your content type (emails, articles, docs)

3. **Severity levels**
   - Mark some patterns as "critical" for your voice
   - Mark others as "watch" (situational)

4. **Detection instructions**
   - Add context about your specific use cases
   - Include edge cases unique to your writing

**Example customization:**

```markdown
## Patterns to Prioritize (For This User)

**Critical violations:**
- Pattern #5: Weak verb substitutions (your biggest gap)
- Pattern #11: Formulaic triplets (you default to three)
- Pattern #24: Vapid closings (watch this in reports)

**Situational:**
- Pattern #6: Passive voice (OK in technical docs, avoid elsewhere)
- Pattern #19: Lists (fine for instructions, not for narratives)
```

---

### Step 5: Integrate into Your Workflow

**Workflow A: Pre-flight Check (Before Publishing)**

1. Write naturally using your voice principles
2. Edit once for clarity and structure
3. Run humanizer skill as final check
4. Address flagged patterns
5. Publish

**Workflow B: Learning Mode (While Building Voice)**

1. Write a draft
2. Run humanizer immediately
3. Study which patterns you hit
4. Revise
5. Repeat until you internalize the patterns

**Workflow C: Spot Check (For High-Stakes Content)**

1. Write using established voice
2. Run humanizer only on critical sections
3. Quick revision
4. Ship

Choose the workflow that matches your skill level and content stakes.

---

### Step 6: Track Your Patterns

Keep notes on which patterns you hit most frequently.

**Tracking template:**

```markdown
## My Pattern Tendencies (Updated: Feb 2026)

**Top violations:**
1. Pattern #11 (Formulaic triplets) — 12 instances this month
2. Pattern #5 (Weak verbs) — 8 instances
3. Pattern #18 (Qualifiers) — 7 instances

**Improving:**
- Pattern #20 (Hedging) — down from 15/month to 3/month
- Pattern #24 (Vapid closings) — caught 100% before publishing

**No longer seeing:**
- Pattern #1 (Long paragraphs) — internalized
- Pattern #8 (Redundancies) — natural now
```

This helps you focus effort on your actual weak spots.

---

## Advanced Integration Strategies

### Strategy 1: Context-Specific Detection

Create versions of the skill for different contexts.

**Example:**

`humanizer-emails.skill` — Emphasizes patterns #21 (filler phrases) and #22 (generic transitions)

`humanizer-articles.skill` — Emphasizes patterns #2 (data dumps) and #24 (vapid closings)

`humanizer-technical.skill` — Allows passive voice, focuses on clarity patterns

### Strategy 2: Team Calibration

If using as a team:

1. Everyone runs their writing through the humanizer
2. Meeting to discuss: Which patterns matter for our brand voice?
3. Customize the skill based on team consensus
4. Share the customized version
5. Quarterly calibration to adjust

### Strategy 3: Before/After Library

Build a personal library of your pattern corrections.

```markdown
## My Pattern Fixes

### Weak Verb Substitutions

Before: "The dashboard serves as a tool for tracking KPIs"
After: "The dashboard tracks KPIs"

Before: "This approach acts as a solution for..."
After: "This approach solves..."
```

This creates a personalized reference faster than reviewing all 24 patterns.

---

## Integration with Other Tools

**Grammarly + Humanizer:**
- Grammarly catches grammar/spelling
- Humanizer catches AI patterns and voice issues
- Run Grammarly first, humanizer second

**Hemingway + Humanizer:**
- Hemingway flags complexity and readability
- Humanizer flags AI patterns
- They complement each other

**Writing Voice Guide + Humanizer:**
- Voice guide defines your positive principles
- Humanizer catches negative patterns
- Use voice guide as primary, humanizer as safety net

---

## When NOT to Use the Humanizer

**Skip pattern detection for:**

1. **First drafts** — Get ideas out first, edit later
2. **Internal notes** — Clarity matters more than polish
3. **Technical specifications** — Some patterns (passive voice, noun clusters) are appropriate
4. **Transcripts or quotes** — Don't edit others' authentic voice
5. **Creative writing** — Intentional pattern-breaking is valid

The humanizer is for professional content where authentic voice matters.

---

## Measuring Success

**You've successfully integrated when:**

- Pattern detection confirms what you already caught (not surprising you)
- Violation count decreases month-over-month
- You internalize patterns and self-correct before detection
- You can explain WHY a pattern matters for YOUR voice, not just that "it's an AI pattern"

**Warning signs of poor integration:**

- Mechanically avoiding patterns without understanding why
- Voice becomes sterile and voiceless
- You're using detection as a crutch instead of building skill
- Every sentence is edited 5+ times trying to eliminate all patterns

Remember: **Authentic voice > Pattern avoidance.**

---

## Customization Examples

### Example 1: Technical Writer

```markdown
## Customized for Technical Documentation

**Patterns to emphasize:**
- #2: Data dumps (organize info better)
- #7: Noun clusters (clarity over compression)
- #10: Misused jargon (precision matters)

**Patterns to de-emphasize:**
- #6: Passive voice (acceptable in procedures)
- #19: Lists (appropriate for instructions)
```

### Example 2: Marketing Content

```markdown
## Customized for Marketing

**Patterns to emphasize:**
- #14: Clichéd metaphors (brand differentiation)
- #22: Generic transitions (specificity sells)
- #24: Vapid closings (CTAs must be concrete)

**Patterns to de-emphasize:**
- #18: Qualifiers (some hedging is prudent)
```

### Example 3: Executive Communications

```markdown
## Customized for Leadership Voice

**Patterns to emphasize:**
- #4: -ing verbs (directness signals authority)
- #5: Weak verbs (be decisive)
- #20: Hedging (confidence matters)

**Patterns to allow:**
- #1: Longer paragraphs (complex ideas need space)
```

---

## Next Steps

1. ✅ Complete your [gap analysis](../methodology/gap-analysis.md)
2. ✅ Document your top 3-5 pattern vulnerabilities
3. ✅ Customize SKILL.md with your examples
4. ✅ Choose your workflow (pre-flight, learning, or spot-check)
5. ✅ Track patterns for one month
6. ✅ Refine customization based on results

## Resources

- [Gap Analysis Methodology](../methodology/gap-analysis.md)
- [Complete Pattern Reference](../humanizer-skill/patterns.md)
- [Installation Guide](installation.md)
- [Before/After Examples](../examples/before-after.md)
