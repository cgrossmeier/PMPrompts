# Prompt: MoSCoW Prioritization Method

## Context
I need to categorize features using the MoSCoW method (Must have, Should have, Could have, Won't have). Help me rigorously classify features into these categories with clear rationale.

## Product Information
**Product**: [Your product]
**Features to Classify**: [List features]
**Release/Scope**: [Timeframe or release version]
**Constraints**: [Fixed deadline, budget, or resources]

## MoSCoW Categories

### Must Have (M)
**Definition:** Non-negotiable requirements without which the product/release fails

**Criteria for Must Have:**
- Legal or regulatory requirement
- Product cannot launch without it
- Core value proposition depends on it
- Critical security or safety issue
- Contractual obligation
- Breaks existing functionality if omitted

**Questions to Ask:**
- What happens if we don't build this?
- Is the release viable without it?
- Is there a workaround?
- Can it wait for next release?

**Must Haves should be:** ~60% or less of total capacity

### Should Have (S)
**Definition:** Important features that add significant value but have workarounds

**Criteria for Should Have:**
- High business value
- Strong customer demand
- Significant pain point solution
- Competitive parity requirement
- Workaround exists but is painful

**Questions to Ask:**
- How painful is the workaround?
- What value is lost without it?
- How many users affected?
- What's the business impact?

**Should Haves should be:** ~20% of total capacity

### Could Have (C)
**Definition:** Nice-to-have features that improve experience but aren't essential

**Criteria for Could Have:**
- Positive but small impact
- Benefits specific use cases
- Polish or convenience features
- Low effort, low risk additions
- Can easily be dropped if needed

**Questions to Ask:**
- Would users miss this?
- Does it solve a real problem?
- Is effort justified by value?
- Could resources be better used?

**Could Haves should be:** ~20% of total capacity

### Won't Have (W)
**Definition:** Features explicitly excluded from this release but may be considered future

**Criteria for Won't Have:**
- Low priority right now
- Out of scope for current goals
- Insufficient resources
- Not aligned with strategy
- Better alternatives exist

**Questions to Ask:**
- Why not now?
- Will it ever be prioritized?
- Should we communicate decision?
- Is it truly won't or shouldn't?

## Classification Process

**Step 1: Initial Categorization**
Assign each feature to a category with initial rationale

**Step 2: Validate Must Haves**
Challenge each Must Have:
- Truly non-negotiable?
- Can release succeed without it?
- Move to Should if not critical

**Step 3: Balance Capacity**
- Calculate total effort for each category
- Must + Should should be ≤80% of capacity
- Could provides buffer for unknowns
- Adjust if categories are imbalanced

**Step 4: Stakeholder Alignment**
- Review classification with stakeholders
- Build consensus on Must vs Should
- Document disagreements and resolution

**Step 5: Define Won't Have**
- Explicitly call out excluded features
- Set expectations for when they might be reconsidered
- Prevent scope creep discussions

## Requested Output

Provide MoSCoW classification:

**Summary Table**
| Category | Feature Count | Total Effort | % of Capacity | Status |
|----------|---------------|--------------|---------------|--------|
| Must Have | [#] | [person-weeks] | [%] | ✓ |
| Should Have | [#] | [person-weeks] | [%] | ✓ |
| Could Have | [#] | [person-weeks] | [%] | ~ |
| Won't Have | [#] | - | - | ✗ |

**Must Have Features**
| # | Feature | Rationale | Effort | Risk |
|---|---------|-----------|--------|------|
| 1 | [Feature] | [Why must have?] | [Est] | [Level] |

**Should Have Features**
| # | Feature | Rationale | Effort | Demotion Trigger |
|---|---------|-----------|--------|------------------|
| 1 | [Feature] | [Why should have?] | [Est] | [When to drop?] |

**Could Have Features**
| # | Feature | Rationale | Effort | Value If Included |
|---|---------|-----------|--------|-------------------|
| 1 | [Feature] | [Why could have?] | [Est] | [Benefit] |

**Won't Have Features**
| # | Feature | Reason for Exclusion | Future Consideration |
|---|---------|---------------------|---------------------|
| 1 | [Feature] | [Why not now?] | [When to revisit?] |

**Capacity Analysis**
- Total capacity: [person-weeks]
- Committed (M+S): [person-weeks] ([%])
- Buffer (C): [person-weeks] ([%])
- **Status**: ✓ Balanced / ⚠ Overcommitted / ✗ Insufficient Buffer

**Risk Assessment**
- Risks to Must Haves
- Contingency plans
- Features to drop if necessary (from Should/Could)

**Stakeholder Communication**
- Key decisions to communicate
- Won't Have features to set expectations on
- Timeline and scope commitments

## Decision Framework

**When to Move Features Between Categories:**

**Must → Should:**
- Found viable workaround
- Reduced business criticality
- Higher effort than expected

**Should → Could:**
- Capacity constraints
- Reduced priority
- Effort increased significantly

**Could → Won't:**
- Insufficient capacity
- Low value relative to alternatives
- Better deferred to future release

**Won't → Should/Could:**
- Strategic change
- Customer escalation
- Capacity freed up

## Review Cadence

**During Planning:**
- Initial classification
- Stakeholder alignment
- Capacity validation

**During Execution:**
- Weekly: Review Could Have inclusion
- Bi-weekly: Reassess Should Haves if at risk
- As needed: Move features based on new information

**Post-Release:**
- Review Won't Have for next release
- Analyze: Did classification work?
- Refine process for next planning

## Additional Context
- **Business Goals**: [Release objectives]
- **Constraints**: [Fixed date, team, budget]
- **Dependencies**: [Features that must go together]
- **Stakeholder Priorities**: [Executive or customer must-haves]
