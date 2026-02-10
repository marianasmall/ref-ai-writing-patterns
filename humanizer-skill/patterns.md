# AI Writing Patterns Reference

Complete catalog of 24 AI writing patterns with explanations and examples.

## How to Use This Reference

Each pattern includes:
- **Description** — What the pattern is
- **Why it matters** — Why AI generates this
- **Examples** — Before (AI pattern) and After (natural)
- **Detection tips** — How to spot it

---

## Category 1: Content & Structure

### Pattern 1: Unnecessarily Long Paragraphs

**Description:** Dense blocks of text without natural breaks for the reader.

**Why AI does this:** Language models optimize for information density rather than readability. They pack related concepts together without considering cognitive load.

**Example:**
- ❌ *[8-sentence paragraph with multiple distinct ideas about project management, team communication, and deadline tracking all merged together]*
- ✅ *[Same content split into 3 paragraphs, each focused on one aspect]*

**Detection:** Count sentences per paragraph. If you regularly exceed 5-6 sentences without intentional design, check if you're packing too much in.

---

### Pattern 2: Data Dumps

**Description:** Listing facts, statistics, or information without context, narrative, or analysis.

**Why AI does this:** Models excel at retrieving and formatting data but struggle with interpretive narrative.

**Example:**
- ❌ "In 2019, revenue was $5M. In 2020, it increased to $6.2M. By 2021, it reached $7.8M. Q1 2022 showed $2.1M."
- ✅ "Revenue grew 24% annually from 2019-2021, maintaining momentum through Q1 2022."

**Detection:** Look for sentence structures that repeat (number-statement, number-statement). Check if data is interpreted or just presented.

---

### Pattern 3: Outdated Information

**Description:** References to events, trends, or data that are no longer current.

**Why AI does this:** Training data cutoffs mean models may reference "recent" events that are now old.

**Example:**
- ❌ "The recent pandemic has changed how we work..." (written in 2026)
- ✅ "Remote work became standard after 2020..."

**Detection:** Check dates, "recent" claims, and references to current events.

---

### Pattern 4: Surface-Level -ing Verbs (Participial Phrases)

**Description:** Using descriptive -ing phrases instead of direct, active language.

**Why AI does this:** Participial phrases feel sophisticated and allow models to layer description, but they create distance from the action.

**Example:**
- ❌ "The platform, symbolizing innovation and reflecting modern needs, transforms collaboration."
- ✅ "The platform transforms how teams collaborate."

**Detection:** Search for commas surrounding -ing phrases. If you can remove the phrase and the sentence improves, it's likely filler description.

---

## Category 2: Language Choices

### Pattern 5: Weak Verb Substitutions

**Description:** Using multi-word phrases like "serves as" or "acts as" instead of direct verbs.

**Why AI does this:** These constructions feel formal and hedge commitment, which models favor for apparent safety.

**Example:**
- ❌ "The tool serves as a solution for team alignment."
- ✅ "The tool solves team alignment." or "The tool is a solution for team alignment."

**Detection:** Search for "serves as," "acts as," "functions as," "works as." Usually a stronger verb or simple "is" works better.

---

### Pattern 6: Passive Voice Overuse

**Description:** Systematically avoiding naming who performs actions.

**Why AI does this:** Passive voice feels neutral and objective, which models interpret as "professional."

**Example:**
- ❌ "The decision was made to proceed with the project."
- ✅ "We decided to proceed with the project."

**Detection:** Look for "was [verb]ed" constructions. Not all passive voice is wrong—use it when the actor truly doesn't matter or is obvious.

---

### Pattern 7: Noun Clusters

**Description:** Stacking multiple nouns together without clear relationships.

**Why AI does this:** Models compress meaning into noun phrases, creating technical-sounding but often unclear language.

**Example:**
- ❌ "customer relationship management system optimization initiatives"
- ✅ "initiatives to optimize how we manage customer relationships"

**Detection:** If you have 3+ nouns in a row, try expanding into a phrase with verbs and prepositions.

---

### Pattern 8: Redundancies

**Description:** Saying the same thing twice in slightly different words.

**Why AI does this:** Models reinforce meaning through repetition, not realizing natural language assumes the reader understood the first time.

**Example:**
- ❌ "past history," "end result," "future plans," "collaborate together"
- ✅ "history," "result," "plans," "collaborate"

**Detection:** Classic redundancies: advance planning, basic fundamentals, close proximity, each individual, final outcome, free gift, past experience, future potential.

---

### Pattern 9: Unnatural Phrasings

**Description:** Constructions that sound AI-generated—technically correct but not how humans naturally express ideas.

**Why AI does this:** Statistical patterns in training data don't always match natural speech rhythms.

**Example:**
- ❌ "It's worth noting that the project succeeded."
- ✅ "The project succeeded."
- ❌ "One might consider exploring alternatives."
- ✅ "Consider alternatives." or "You might explore alternatives."

**Detection:** Read aloud. If you wouldn't say it in conversation with a colleague, it's likely unnatural.

---

### Pattern 10: Misused Jargon

**Description:** Using technical terms incorrectly or where simpler language would be clearer.

**Why AI does this:** Models associate technical terms with expertise but don't always understand correct usage contexts.

**Example:**
- ❌ Using "leverage" for "use," "utilize" for "use," "paradigm" incorrectly
- ✅ Using precise terms only when necessary

**Detection:** For every technical term, ask: "Could I say this more simply? Does this term add meaning or just sound fancy?"

---

## Category 3: Style Markers

### Pattern 11: Formulaic Triplets (Rule of Three)

**Description:** Always grouping ideas, examples, or concepts in threes.

**Why AI does this:** The rule of three is taught as a rhetorical device, so models overuse it.

**Example:**
- ❌ "Innovation, inspiration, and implementation drive success."
- ✅ Use the natural count: "Two forces drive success: X and Y" or "Four principles guide us: A, B, C, D"

**Detection:** Count groupings. If everything comes in threes, you're forcing patterns.

---

### Pattern 12: Title Case Overuse

**Description:** Capitalizing ordinary concepts to make them seem important.

**Why AI does this:** Models interpret capitals as signaling importance but overdo it.

**Example:**
- ❌ "Our Strategy for Growth and Innovation"
- ✅ "our strategy for growth and innovation"

**Detection:** Only capitalize proper nouns, titles (when used as titles), and sentence beginnings.

---

### Pattern 13: Robotic Transitions

**Description:** Mechanical, repetitive connectors between ideas.

**Why AI does this:** Models explicitly signal transitions rather than letting ideas flow naturally.

**Example:**
- ❌ "Furthermore, the data shows... Moreover, this indicates... In addition, we found..."
- ✅ Vary transitions or let the relationship be implied. "The data shows... This indicates... We also found..."

**Detection:** Count "furthermore," "moreover," "additionally," "in addition." More than one per page is usually too many.

---

### Pattern 14: Clichéd Metaphors

**Description:** Overused comparisons and figures of speech.

**Why AI does this:** These appear frequently in training data, so models treat them as high-quality expressions.

**Example:**
- ❌ "tip of the iceberg," "paradigm shift," "game changer," "low-hanging fruit," "move the needle"
- ✅ Create fresh comparisons or state directly: "This solves 10% of the problem—the easier part."

**Detection:** If you've heard the metaphor in business meetings repeatedly, it's cliché.

---

### Pattern 15: Uniform Sentence Structure

**Description:** Every sentence following the same grammatical pattern.

**Why AI does this:** Models default to subject-verb-object constructions without natural rhythm variation.

**Example:**
- ❌ "The team completed the project. The client approved the results. The manager scheduled follow-up. The stakeholders reviewed documentation."
- ✅ "The team completed the project, and the client approved it. After scheduling a follow-up, the manager had stakeholders review the documentation."

**Detection:** Read aloud. Does it sound monotonous? Vary sentence length and structure deliberately.

---

### Pattern 16: Comma Splices

**Description:** Incorrectly joining independent clauses with only a comma.

**Why AI does this:** Models sometimes compress related ideas without proper punctuation.

**Example:**
- ❌ "The project was delayed, the team worked overtime."
- ✅ "The project was delayed, so the team worked overtime." or "The project was delayed. The team worked overtime."

**Detection:** If you can replace the comma with a period and get two complete sentences, you likely need a stronger connector or a semicolon.

---

### Pattern 17: False Scope Ranges

**Description:** Claiming to cover more breadth than actually addressed.

**Why AI does this:** Models aim for comprehensive-sounding language even when content is narrow.

**Example:**
- ❌ "Covering everything from basic setup to enterprise architecture" [when only discussing mid-level features]
- ✅ "Covering setup, team workflows, and deployment to production"

**Detection:** Check if "from X to Y" accurately represents the full range of content. Be specific about what's actually included.

---

## Category 4: Communication Patterns

### Pattern 18: Unnecessary Qualifiers

**Description:** Weakening statements with excessive modifiers that add no meaning.

**Why AI does this:** Models hedge to avoid appearing overconfident.

**Example:**
- ❌ "This approach is somewhat effective and quite useful in fairly common situations."
- ✅ "This approach works in common situations."

**Detection:** Remove "somewhat," "quite," "rather," "fairly," "relatively," "arguably" and see if meaning changes. Usually it doesn't.

---

### Pattern 19: Listiness

**Description:** Over-reliance on bullet points and numbered lists when prose would be more natural.

**Why AI does this:** Lists are easy for models to generate and appear organized.

**Example:**
- ❌ Using bullets for everything, even simple concepts that should be a sentence
- ✅ Use lists for actual lists; use prose for ideas, explanations, and narratives

**Detection:** If you're creating a list, ask: "Would this be clearer as 2-3 sentences?"

---

### Pattern 20: Excessive Hedging

**Description:** Too many disclaimers and qualifying phrases.

**Why AI does this:** Models prioritize appearing measured and avoiding strong claims.

**Example:**
- ❌ "It might be possible that one could perhaps consider exploring..."
- ✅ "Consider exploring..." or "You could explore..."

**Detection:** Count hedge words: might, perhaps, possibly, potentially, could, may. More than one per paragraph deserves scrutiny.

---

### Pattern 21: Filler Phrases

**Description:** Empty language that adds no meaning or information.

**Why AI does this:** These phrases appear frequently in training data and models use them as sentence starters.

**Examples:**
- ❌ "It's important to note that..."
- ❌ "It should be emphasized that..."
- ❌ "As a matter of fact..."
- ❌ "At the end of the day..."
- ❌ "When it comes to..."
- ✅ Just state the thing directly

**Detection:** If you can delete the phrase and the sentence improves, it was filler.

---

### Pattern 22: Generic Transitions

**Description:** Cookie-cutter phrases that could apply to any topic.

**Why AI does this:** These provide safe, universal connectors without requiring specific understanding.

**Example:**
- ❌ "In today's fast-paced world," "In an increasingly digital landscape," "As we move forward"
- ✅ Be specific: "Since remote work became standard," "With the rise of mobile-first design"

**Detection:** Could this phrase apply to any industry or topic? If yes, it's too generic.

---

### Pattern 23: Overuse of Latin/Greek Affixes

**Description:** Adding -ize, -ification, -ation unnecessarily.

**Why AI does this:** These suffixes make words sound formal and technical.

**Example:**
- ❌ "utilization of resources" → "use of resources" or "using resources"
- ❌ "optimization of processes" → "improving processes"
- ❌ "finalization of plans" → "finalizing plans"

**Detection:** For words ending in -ization, -ification, -ation, check if a simpler form exists.

---

## Category 5: Filler & Hedging

### Pattern 24: Vapid Closings

**Description:** Generic endings with no substance or specificity.

**Why AI does this:** Models generate wrap-up language when uncertain how to conclude.

**Examples:**
- ❌ "The future looks bright for AI-powered marketing."
- ❌ "Only time will tell how this develops."
- ❌ "It remains to be seen what will happen next."
- ❌ "The possibilities are endless."
- ✅ End with: specific next step, concrete data point, or thought-provoking observation

**Detection:** Does your closing say something meaningful, or could it end any article on any topic?

---

## Using This Reference

**For detection:**
Keep this list handy when reviewing content. Check for patterns that appear frequently in your writing.

**For improvement:**
Focus on your top 3-5 patterns first. Learn to self-correct these, then move to others.

**For context:**
Remember: these are patterns, not rules. Some legitimate writing triggers these flags. The goal is authentic voice, not mechanical pattern avoidance.

---

## Credits

Pattern catalog sourced from Wikipedia's "Signs of AI Writing" article, maintained by WikiProject AI Cleanup.

This reference created February 2026 as part of the [AI Writing Patterns](https://github.com/marianasmall/ai-writing-patterns) project.
