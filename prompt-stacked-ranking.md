# Prompt: Stacked Ranking for Feature Prioritization

## Context
I need to create a forced-ranking of all features where each feature has a unique position from #1 to #N. This eliminates ties and forces difficult trade-off decisions.

## Product Information
**Product**: [Your product]
**Features to Rank**: [List features]
**Ranking Criteria**: [Primary decision factors]

## Stacked Ranking Methodology

### Core Principle
Every feature must have a unique rank. No ties allowed. Forces explicit prioritization decisions.

### Ranking Criteria

Weight each criterion based on strategic priorities:

**Business Value** (Weight: __%)
- Revenue impact (new, expansion, retention)
- Strategic alignment
- Market opportunity size
- Competitive positioning

**Customer Impact** (Weight: __%)
- Number of users affected
- Severity of problem solved
- Frequency of use
- Customer delight potential

**Effort & Feasibility** (Weight: __%)
- Development time required
- Technical complexity
- Team capability/availability
- Risk level

**Urgency & Timing** (Weight: __%)
- Market window
- Contractual commitments
- Dependencies on other work
- Competitive pressure

## Ranking Process

**Step 1: Initial Scoring**
Score each feature (1-10) on each criterion

**Step 2: Weighted Score**
Calculate: Sum of (Criterion Score × Weight)

**Step 3: Initial Ranking**
Rank by weighted score (highest to lowest)

**Step 4: Pairwise Comparison**
For adjacent features, ask:
"If we could only build one, which would it be?"
Swap positions if needed based on answer

**Step 5: Forced Choices**
For any remaining uncertainty:
- Force explicit trade-off decisions
- Document rationale
- No "both are equal" allowed

**Step 6: Validation**
Review top 10 and bottom 10:
- Does ranking feel right?
- Challenge scoring if counterintuitive
- Adjust and re-rank if needed

## Stakeholder Alignment

**Individual Rankings**
Have key stakeholders do independent rankings

**Consolidated Ranking**
- Average rankings across stakeholders
- Discuss major discrepancies (>5 rank difference)
- Build consensus through debate
- Use executive decision-maker for final ties

## Requested Output

**Final Stacked Ranking**
| Rank | Feature | Weighted Score | Business Value | Customer Impact | Effort | Urgency | Rationale |
|------|---------|----------------|----------------|-----------------|--------|---------|-----------|
| 1 | [Feature] | 8.7 | 9 | 9 | 7 | 9 | [Why #1?] |
| 2 | [Feature] | 8.5 | 8 | 9 | 8 | 8 | [Why #2?] |
| ... | ... | ... | ... | ... | ... | ... | ... |

**Top 10 Analysis**
Detailed rationale for top 10 features including:
- Why this rank vs. alternatives?
- Key trade-offs made
- Confidence level in ranking
- Dependencies or sequencing needs

**Bottom Quartile Review**
- Why ranked low?
- Reconsider or eliminate?
- Future potential?

**Stakeholder Comparison**
| Feature | Your Rank | Stakeholder A | Stakeholder B | Variance | Consensus |
|---------|-----------|---------------|---------------|----------|-----------|

**Sequencing Plan**
Given ranking, recommended execution sequence considering:
- Resource availability
- Dependencies
- Quick wins for momentum
- Risk diversification

**Cutline Analysis**
For given capacity (e.g., 10 features):
- What falls above/below the line?
- What's the marginal value of #11?
- What would change to include #11?

## Ranking Challenges

**Common Pitfalls:**

**Clustering Near the Top**
- Forces real differentiation in top 10
- No "everything is priority 1"

**Effort Bias**
- Don't over-weight easy features
- High value, high effort can be worth it

**Recency Bias**
- Recent feedback over-emphasized
- Balance with strategic view

**HIPPO Effect**
- Highest paid person's opinion
- Data and frameworks counter this

## Dynamic Re-ranking

**Triggers to Re-rank:**
- Quarterly planning cycles
- Significant new information
- Strategic pivot
- Competitive changes
- Technical discoveries

**Between Re-ranks:**
- Adjust +/-3 positions max
- Document rationale
- Communicate changes

## Tie-Breaking Rules

When features score identically:

1. **Strategic Alignment**: More aligned wins
2. **Customer Impact**: More users wins
3. **Risk**: Lower risk wins
4. **Time to Value**: Faster wins
5. **Executive Decision**: Final call

## Visualization

**Ranked List with Indicators**
```
🔴 #1  [Feature] - Strategic Imperative
🔴 #2  [Feature] - Quick Win
🟡 #3  [Feature] - High Effort
🟡 #4  [Feature] - Dependency Risk
🟢 #5  [Feature] - Customer Request
...
⚪ #20 [Feature] - Deprioritized
```

**Scoring Heatmap**
Visual showing score distribution across criteria

**Confidence Bands**
- High confidence (scores >2 points apart)
- Medium confidence (1-2 points apart)
- Low confidence (<1 point apart - needs review)

## Roadmap Translation

**Q1 Execution** (Ranks 1-5)
Resource allocation and timeline

**Q2 Planning** (Ranks 6-12)
Preparation and dependencies

**Q3+ Consideration** (Ranks 13+)
Monitor and re-evaluate

## Additional Context
- **Capacity Constraints**: [How many features can be built?]
- **Strategic Mandates**: [Any must-dos regardless of rank?]
- **Team Composition**: [Skills available affecting feasibility?]
- **Market Timing**: [Time-sensitive opportunities?]
