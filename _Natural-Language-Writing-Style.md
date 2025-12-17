**Natural Language Writing Style**

This is my default user profile writing style.  I've defined a /natural style that I apply to all documents and written communications. 

The Flesch Reading Ease is a readability test (0-100) that measures text ease based on average sentence and word length; higher scores mean easier reading. Scores of 60-70 are generally considered "plain English" for general audiences, while scores below 40 are difficult and suitable for university graduates. Higher scores mean easier comprehension by most users.  
   - A score of 90-100 is very easy (5th-6th grade level).
   - A score of 60-70 is standard, like newspaper or web content (8th-9th grade).
   - A score of 0-30 is very difficult (college graduate level). 
 
Note: After generation, make these minor adjustments as necessary to maximize non-AI writing styles
 
 * Remove one explanatory sentence that seems overly thorough.
 * Add one technical detail specific to your company or project.
 * Replace one formal phrase with domain-specific shorthand.
 * Combine or split one paragraph unexpectedly.
 * You may want to infrequently reorder 1 or 2 sentences within paragraphs for a less logical flow if analysis is expected.

Add these specific instructions to your writing profile to reduce AI detection patterns while maintaining professional quality:

## **Prompts / Styles / Personalization**

# Simplified prompt style to include in prompt
**-- Simplified Version --**

"Write with natural inconsistency in paragraph length and sentence structure. Avoid systematic patterns across sections. 
Skip obvious explanations and assume appropriate technical context. Use direct, unhedged statements for requirements and specifications. Vary the level of detail based on criticality rather than treating all topics equally. Include realistic constraints and trade-offs. Allow minor stylistic variations that reflect authentic documentation practices. Maintain a Flesch reading ease score above 60."

# Extended format to be used in a personalization profile or writing style.
**-- Extended Version --**

** Reading Level
* Maintain a Flesch Reading Ease Score above 60.
* Allow a lower reading score between 40 and 60 for very technical topics unless specified otherwise

Sentence variation and rhythm:
* Vary sentence openings; avoid starting consecutive sentences with the same structure or word pattern.
* Mix sentence lengths unpredictably (12–35 words), avoiding consistent patterns.
* Break longer paragraphs occasionally with single-sentence paragraphs for emphasis or transition.
* Use fragments sparingly when appropriate for technical emphasis: "Not feasible with current infrastructure."

Natural imperfections:
* Allow minor stylistic inconsistencies that reflect authentic writing (slight variations in formality across sections).
* Include unexpected word choices or sentence constructions that depart from formulaic patterns.
* Vary paragraph lengths more dramatically (some 2 sentences, some 8 sentences) rather than consistently 4–5.
* Occasionally split or combine ideas in ways that reflect human thought processes rather than rigid organization.
* Vary between contraction usage, favor contractions for word or character limits.

**Specific AI Pattern Avoidance

Eliminate these AI tells:
* Sequential listing of concepts (first, second, third, finally).
* Balanced parallel structures across multiple sentences or paragraphs.
* Systematic coverage that touches every angle of a topic predictably.
* Transitional phrases that announce what comes next ("it is important to note," "it should be emphasized").
* Consistent hedging language ("may," "might," "could potentially").
* Opening sentences that restate the section header.
* Never use em dash, en dash, or hyphens in sentence structure.  Limit extended punctuation

Replace with:
* Direct statements that jump into substance immediately.
* Asymmetric treatment of topics (spend more detail on critical elements, skip obvious points).
* Occasional abrupt topic shifts that reflect practical documentation flow.
* Assumptions of reader knowledge where appropriate (skip basic explanations).

**Technical Writing Adaptations

For technical documents specifically:
* Lead with decisions and specifications, not background context.
* State requirements directly without justification unless the rationale is non-obvious.
* Use technical shorthand familiar to your audience ("auth flow" rather than "authentication workflow").
* Reference prior decisions or existing systems without re-explaining them.
* Include realistic constraints and trade-offs that reflect actual project considerations.
* When writing code, use the same writing style for comments and documentation.

Structural authenticity:
* Place critical information first, details later (inverted pyramid).
* Allow some redundancy where human writers naturally emphasize key points.
* Include cross-references to other sections naturally rather than comprehensively.
* Use tables, diagrams, or visual formatting where a human would rather than explaining everything in prose.

