# Prompt: RICE Scorecard for Product Prioritization

## Context
I need to score and prioritize features using the RICE framework (Reach × Impact × Confidence / Effort). Help me systematically evaluate each feature across these four dimensions.

## Product Information
**Product**: [Your product]
**Features to Score**: [List features]
**Time Period**: [Typically quarterly or per release]

## RICE Scoring Framework

For each feature, evaluate:

### Reach
**How many users/customers will this impact per time period?**

Measure specific to your context:
- Monthly active users who will use this feature
- Customers affected in target segment
- Transactions/sessions impacted
- Support tickets resolved

**Reach Score**: [Number of people/events per period]

Tips for estimation:
- Use analytics data for existing features
- Benchmark similar feature adoption rates
- Consider funnel percentages
- Segment by user type if relevant

### Impact
**How much will this impact each person/event when they encounter it?**

Score on standardized scale:
- **3 = Massive impact** - Transforms experience, solves critical pain
- **2 = High impact** - Significant improvement, strong value
- **1 = Medium impact** - Notable improvement, decent value
- **0.5 = Low impact** - Small improvement, minor value
- **0.25 = Minimal impact** - Barely noticeable improvement

**Impact Score**: [0.25, 0.5, 1, 2, or 3]

Consider:
- How painful is the problem being solved?
- How much better is the new experience?
- What is the value delivered?
- Would users actively seek this?

### Confidence
**How certain are you about your Reach and Impact estimates?**

Score as percentage:
- **100% = High confidence** - Strong data, validated assumptions
- **80% = Medium confidence** - Reasonable data, some validation
- **50% = Low confidence** - Estimates, limited data

**Confidence Score**: [50%, 80%, or 100%]

Be honest about uncertainty:
- Do you have user research backing this?
- Are there analytics or market data?
- Have you tested prototypes?
- How novel is this feature?

### Effort
**How many person-months will this take to build?**

Include all work:
- Engineering development time
- Design and UX work
- Product management
- QA and testing
- Documentation and deployment

**Effort Score**: [Person-months]

Tips for estimation:
- Include full team effort (not just engineering)
- Add buffer for unknowns (multiply by 1.2-1.5)
- Consider technical debt paydown
- Account for dependencies

## RICE Score Calculation

**RICE Score = (Reach × Impact × Confidence) / Effort**

Example:
- Feature reaches 10,000 users/month
- Impact score of 2 (high impact)
- Confidence of 80%
- Effort of 4 person-months
- RICE = (10,000 × 2 × 0.8) / 4 = 4,000

Higher RICE score = higher priority

## Requested Output

Provide comprehensive RICE analysis:

**RICE Scorecard Table**
| Feature | Reach | Impact | Confidence | Effort | RICE Score | Rank |
|---------|-------|--------|------------|--------|------------|------|
| Feature 1 | 10,000 | 2 | 80% | 4 | 4,000 | 1 |
| Feature 2 | ... | ... | ... | ... | ... | ... |

**Prioritized Feature List**
Features ranked by RICE score with rationale for top priorities

**Scoring Rationale**
Detailed explanation for each score:
- Why this Reach estimate?
- What drives this Impact level?
- What creates this Confidence level?
- How was Effort estimated?

**Sensitivity Analysis**
How ranking changes if key assumptions vary (especially low-confidence items)

**Portfolio Balance Review**
- Mix of quick wins (low effort) vs big bets (high reach)
- Confidence level distribution
- Resource allocation across quarters

**Roadmap Recommendation**
Sequencing based on RICE scores, dependencies, and strategic timing

## Calibration Guidelines

**Normalizing Reach across different metrics:**
If some features impact users and others impact transactions:
- Convert to common unit (e.g., "value units")
- Or score categories separately, then combine

**Impact calibration:**
- Define clear examples for each impact level
- Calibrate across team to ensure consistency
- Use past features as benchmarks

**Confidence calibration:**
- Default to 80% unless strong reasons for higher/lower
- Lower confidence for novel ideas
- Higher confidence for proven patterns

**Effort calibration:**
- Use historical velocity data
- Compare to similar past features
- Include full team effort

## Additional Context
- **Strategic Priorities**: [How should strategy influence scoring?]
- **Resource Constraints**: [Team capacity per quarter]
- **Dependencies**: [Features that must go together]
- **Time Sensitivity**: [Market timing or competitive factors]
