# Prompt: Kano Model for Feature Prioritization

## Context
I need to categorize features using the Kano Model to understand how each feature's presence or absence affects customer satisfaction. This helps identify which features create delight, which prevent dissatisfaction, and which customers don't care about.

## Product Information
**Product**: [Your product]
**Features to Evaluate**: [List features]
**Target Customers**: [Segment to analyze]
**Survey Size**: [Number of customers to survey]

## Kano Survey Design

For each feature, ask customers two questions:

**Functional Question** (feature present):
"How would you feel if [feature description] was available?"

**Dysfunctional Question** (feature absent):
"How would you feel if [feature description] was NOT available?"

**Response Options** (both questions):
1. I like it that way
2. I expect it that way
3. I am neutral
4. I can tolerate it that way
5. I dislike it that way

## Kano Classification Matrix

Cross-tabulate responses to categorize each feature:

| Dysfunctional → <br> Functional ↓ | Like | Expect | Neutral | Tolerate | Dislike |
|---|---|---|---|---|---|
| **Like** | Q | E | E | E | P |
| **Expect** | R | I | I | I | M |
| **Neutral** | R | I | I | I | M |
| **Tolerate** | R | I | I | I | M |
| **Dislike** | R | R | R | R | Q |

**Categories:**
- **M** = Must-Be (Basic Need)
- **P** = Performance (One-Dimensional)
- **E** = Excitement (Delighter)
- **I** = Indifferent
- **R** = Reverse
- **Q** = Questionable (inconsistent response)

## Feature Categories

**Must-Be Features (Basic Needs)**
- Customers expect these; don't praise when present
- Major dissatisfaction when absent
- Examples: Security, reliability, core functionality
- **Strategy**: Must include; table stakes

**Performance Features (One-Dimensional)**
- Satisfaction increases linearly with quality
- More/better = more satisfaction
- Examples: Speed, accuracy, capacity
- **Strategy**: Competitive differentiator; continuous improvement

**Excitement Features (Delighters)**
- Customers don't expect; create delight when present
- No dissatisfaction when absent
- Examples: Unexpected innovations, proactive features
- **Strategy**: Differentiation opportunity; competitive moat

**Indifferent Features**
- Presence or absence doesn't affect satisfaction
- Examples: Rarely-used customization, esoteric settings
- **Strategy**: Deprioritize; waste of resources

**Reverse Features**
- Some customers prefer absence
- Examples: Complexity, excessive options
- **Strategy**: Remove or segment

## Kano Analysis

For each feature, calculate:

**Category Distribution:**
Count responses in each category (M, P, E, I, R)
- Primary category = most frequent response
- Consider splitting if responses are mixed

**Satisfaction Coefficient:**
- **Positive Impact** = (E + P) / (E + P + M + I)
- **Negative Impact** = -1 × (M + P) / (E + P + M + I)
- Closer to +1 = more positive satisfaction impact
- Closer to -1 = more negative if absent

**Category Evolution:**
Consider where features are in lifecycle:
- E → P → M over time as markets mature
- Plan for tomorrow's Must-Bes

## Requested Output

Provide comprehensive Kano analysis:

**Feature Classification Table**
| Feature | Must-Be % | Performance % | Excitement % | Indifferent % | Primary Category | Satisfaction Impact |
|---------|-----------|---------------|--------------|---------------|------------------|---------------------|

**Category Summary**
- Must-Be Features: [List with rationale]
- Performance Features: [List with rationale]
- Excitement Features: [List with rationale]
- Indifferent Features: [List with rationale]
- Reverse Features: [List with rationale]

**Kano Diagram**
Visual plot showing satisfaction vs implementation:
- E features: steep positive, flat without
- P features: diagonal line
- M features: flat with, steep negative without

**Prioritization Strategy**

1. **Immediate Priorities** (avoid dissatisfaction):
   - Must-Be features currently missing
   - Critical Performance features below competitive parity

2. **Differentiation Opportunities** (create delight):
   - Excitement features to build
   - Performance features to excel at

3. **Efficiency Gains** (eliminate waste):
   - Indifferent features to remove
   - Reverse features to eliminate

**Roadmap Implications**
- Balance Must-Bes (hygiene) with Excitement (differentiation)
- Selective investment in Performance (competitive positioning)
- Remove or simplify Indifferent features

**Evolution Planning**
- Which Excitement features are becoming Performance?
- Which Performance features are becoming Must-Be?
- Where to invest in tomorrow's delighters?

## Survey Recommendations

**Sample Size:**
- Minimum 20-30 responses per segment
- More for mixed or uncertain results

**Segmentation:**
- Run separate analysis for different customer types
- Categories may vary by segment

**Frequency:**
- Annual review as markets evolve
- After major product changes

## Additional Context
- **Current Feature State**: [Which features exist today?]
- **Competitive Context**: [What do competitors offer?]
- **Strategic Focus**: [Innovation vs. parity vs. basics?]
- **Resource Constraints**: [What can realistically be built?]
