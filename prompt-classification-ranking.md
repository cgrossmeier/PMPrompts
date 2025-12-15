# Prompt: Classification Ranking for Feature Prioritization

## Context
I need to classify features into distinct priority buckets based on strategic value, then rank within each bucket. This creates clear prioritization tiers while maintaining flexibility within tiers.

## Product Information
**Product**: [Your product]
**Features to Classify**: [List features]
**Planning Horizon**: [Quarter, release, or year]

## Classification Buckets

Define 3-5 classification buckets based on strategic criteria:

### Tier 1: Strategic Imperatives
**Criteria:**
- Direct impact on company OKRs
- Competitive differentiation
- Executive-sponsored initiatives
- Board commitments
- Market-defining opportunities

**Allocation Target**: 20-30% of features

### Tier 2: High-Value Enhancements
**Criteria:**
- Strong customer demand
- Measurable business impact
- Addresses known pain points
- Improves core value proposition
- Enables expansion revenue

**Allocation Target**: 30-40% of features

### Tier 3: Quality and Polish
**Criteria:**
- UX improvements
- Performance optimization
- Technical debt reduction
- Support cost reduction
- Minor enhancements

**Allocation Target**: 20-30% of features

### Tier 4: Maintenance and Operations
**Criteria:**
- Bug fixes
- Infrastructure updates
- Compliance requirements
- Security patches
- Platform upgrades

**Allocation Target**: 10-20% of features

### Tier 5: Nice-to-Haves
**Criteria:**
- Low impact improvements
- Experimental features
- Edge case solutions
- Spare capacity projects

**Allocation Target**: 0-10% of features

## Classification Process

**Step 1: Define Criteria**
Customize bucket criteria to your strategic priorities

**Step 2: Initial Classification**
Place each feature in appropriate bucket based on criteria

**Step 3: Validate Distribution**
- Check allocation percentages
- Rebalance if needed
- Challenge Tier 1 features (truly strategic?)

**Step 4: Rank Within Buckets**
For each bucket, rank features by:
- Business value
- Customer impact
- Effort required
- Dependencies
- Risk

**Step 5: Sequence Across Buckets**
- Tier 1 gets priority in resource allocation
- Balance quick wins vs. strategic bets
- Maintain capacity for Tier 4 (operations)

## Ranking Criteria Within Buckets

**Value Scoring (1-10):**
- Revenue impact
- Customer satisfaction
- Strategic alignment
- Competitive positioning
- Market timing

**Effort Scoring (1-10, lower is less effort):**
- Development time
- Complexity
- Dependencies
- Risk level
- Team availability

**Priority Score = Value / Effort**

Higher score = higher priority within bucket

## Requested Output

Provide classification and ranking:

**Portfolio Overview**
| Tier | Count | Effort | % Capacity | Target % |
|------|-------|--------|-----------|----------|
| 1: Strategic | [#] | [weeks] | [%] | 20-30% |
| 2: High-Value | [#] | [weeks] | [%] | 30-40% |
| 3: Quality | [#] | [weeks] | [%] | 20-30% |
| 4: Maintenance | [#] | [weeks] | [%] | 10-20% |
| 5: Nice-to-Have | [#] | [weeks] | [%] | 0-10% |

**Tier 1: Strategic Imperatives**
| Rank | Feature | Value | Effort | Priority | Rationale |
|------|---------|-------|--------|----------|-----------|
| 1 | [Feature] | 9 | 3 | 3.0 | [Why Tier 1?] |

**Tier 2: High-Value Enhancements**
| Rank | Feature | Value | Effort | Priority | Impact |
|------|---------|-------|--------|----------|--------|

**Tier 3: Quality and Polish**
| Rank | Feature | Value | Effort | Priority | Benefit |
|------|---------|-------|--------|----------|---------|

**Tier 4: Maintenance and Operations**
| Rank | Feature | Value | Effort | Priority | Necessity |
|------|---------|-------|--------|----------|-----------|

**Tier 5: Nice-to-Haves**
| Rank | Feature | Value | Effort | Priority | Condition |
|------|---------|-------|--------|----------|-----------|

**Sequencing Recommendation**
Quarter-by-quarter or release-by-release plan showing:
- Mix of tiers in each period
- Dependencies and sequencing
- Resource allocation
- Risk mitigation

**Portfolio Balance Analysis**
- Strategic vs. tactical balance
- Innovation vs. maintenance balance
- Quick wins vs. long-term bets
- Risk distribution

**Classification Rationale**
Detailed explanation for tier assignment of top features

## Flexibility Rules

**Promotion Triggers:**
Move features up a tier if:
- Strategic priority changes
- Customer escalation
- Competitive threat
- Market opportunity

**Demotion Triggers:**
Move features down a tier if:
- Reduced business value
- Increased complexity
- Resource constraints
- Better alternatives found

**Cross-Tier Dependencies:**
- Handle dependencies that span tiers
- Elevate lower-tier dependencies if blocking higher tiers

## Review Process

**Monthly Review:**
- Validate tier assignments
- Adjust for new information
- Rebalance portfolio if needed

**Quarterly Planning:**
- Refresh entire classification
- Update strategic priorities
- Realign with company goals

## Additional Context
- **Strategic Priorities**: [Company OKRs and goals]
- **Resource Capacity**: [Available team capacity]
- **Market Context**: [Competitive or timing pressures]
- **Technical Constraints**: [Platform or dependency limitations]
