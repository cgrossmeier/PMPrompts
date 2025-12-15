# Prompt: Generate 25 Product Enhancement Ideas

## Context
I need to generate creative, data-informed enhancement ideas for my product. For each idea, provide priority rank, risk assessment, cost estimate, and value to the product.

## Product Information
**Product Name**: [Your product]
**Product Description**: [What does it do, who uses it, key capabilities]
**Current Version/State**: [Where the product is today]
**Target Market**: [Primary customer segments]
**Key Competitors**: [Main alternatives customers consider]
**Strategic Goals**: [What the company is trying to achieve]
**Known Pain Points**: [Current user frustrations or limitations]
**Recent Feedback**: [Customer requests or complaints]

## Enhancement Generation Framework

Generate 25 distinct enhancement ideas across these categories:

**Category Distribution:**
- Core Feature Enhancements (8 ideas): Improvements to existing major features
- New Capabilities (5 ideas): Novel features that expand product value
- UX & Usability (4 ideas): Interface and experience improvements
- Performance & Reliability (3 ideas): Speed, scale, and quality improvements
- Integration & Ecosystem (2 ideas): Connections with other tools
- Platform & Infrastructure (2 ideas): Technical foundation improvements
- AI/ML Enhancements (1 idea): Intelligent or automated capabilities

## Requested Output Format

For each enhancement idea, provide:

| # | Category | Enhancement Idea | Priority | Risk | Cost | Value | Rationale |
|---|----------|------------------|----------|------|------|-------|-----------|

**Field Definitions:**

**Enhancement Idea**: 
Clear, concise description of the enhancement (1-2 sentences)

**Priority Rank**: 
Scale 1-5 where:
- 5 = Critical - Should be immediate focus
- 4 = High - Should be in next release
- 3 = Medium - Important but can wait
- 2 = Low - Nice to have
- 1 = Minimal - Only if spare capacity

Based on: strategic fit + customer impact + competitive need

**Risk Level**:
Scale 1-5 where:
- 5 = Very High Risk - Uncertain feasibility, major technical challenges
- 4 = High Risk - Significant complexity or unknowns
- 3 = Medium Risk - Moderate challenges, some unknowns
- 2 = Low Risk - Well-understood, proven approach
- 1 = Minimal Risk - Straightforward, low complexity

Consider: technical complexity, market uncertainty, execution risk

**Cost Estimate**:
Scale 1-5 where:
- 5 = Very High Cost - 6+ person-months, significant resources
- 4 = High Cost - 3-6 person-months
- 3 = Medium Cost - 1-3 person-months
- 2 = Low Cost - 2-4 person-weeks
- 1 = Minimal Cost - Under 2 weeks

Include: design, engineering, QA, documentation, infrastructure

**Value to Product**:
Scale 1-5 where:
- 5 = Transformative - Game-changing competitive advantage
- 4 = High Value - Significant differentiation or revenue impact
- 3 = Medium Value - Notable improvement in key area
- 2 = Low Value - Incremental improvement
- 1 = Minimal Value - Small polish or edge case

Consider: revenue impact, competitive position, customer satisfaction, strategic alignment

**Rationale**:
1-2 sentences explaining the opportunity and impact

## Example Enhancements

### Core Feature Enhancements
1. **Advanced Filtering**: Multi-criteria filtering with saved filter presets (Priority: 4, Risk: 2, Cost: 3, Value: 4) - Customers frequently request ability to filter by multiple dimensions simultaneously. High ROI given strong demand and moderate effort.

### New Capabilities  
10. **Collaborative Workspaces**: Real-time multiplayer editing and commenting (Priority: 4, Risk: 4, Cost: 5, Value: 5) - Enterprise customers need collaboration. High value but complex technical implementation requiring WebRTC/CRDT.

### UX & Usability
15. **Onboarding Wizard**: Guided 3-step setup flow for new users (Priority: 5, Risk: 2, Cost: 2, Value: 4) - Activation rate currently low. Simple implementation, high impact on conversion.

### Performance & Reliability
18. **Response Caching**: Implement Redis caching for common queries (Priority: 4, Risk: 2, Cost: 3, Value: 4) - P95 latency too high. Well-understood solution with significant performance gains.

### Integration & Ecosystem
21. **Slack Integration**: Two-way sync with notifications and commands (Priority: 3, Risk: 2, Cost: 3, Value: 3) - Frequently requested. Standard integration pattern, broadens appeal.

### Platform & Infrastructure
23. **API Rate Limiting**: Implement token bucket algorithm (Priority: 4, Risk: 2, Cost: 2, Value: 3) - Needed for fairness and abuse prevention. Essential for scale.

### AI/ML Enhancements
25. **Smart Suggestions**: ML-powered recommendations based on usage patterns (Priority: 3, Risk: 4, Cost: 4, Value: 4) - Could differentiate product significantly. Requires data science investment.

## Analysis Summary

After generating 25 ideas, provide:

**Priority Distribution:**
- Priority 5 (Critical): [count]
- Priority 4 (High): [count]
- Priority 3 (Medium): [count]
- Priority 2-1 (Low): [count]

**Value-to-Cost Ratio:**
Top 5 ideas by Value/Cost ratio

**Quick Wins:**
Ideas with Priority ≥3, Risk ≤2, Cost ≤2

**Strategic Bets:**
Ideas with Priority ≥4, Value ≥4, regardless of cost/risk

**Recommended Roadmap:**
Top 10 ideas for next 6-12 months with sequencing rationale

**Portfolio Balance:**
- Innovation vs. optimization
- Customer-driven vs. strategic
- Quick wins vs. long-term bets

## Additional Context
- **Competitive Intelligence**: [What are competitors shipping?]
- **Customer Feedback Themes**: [Top requested features]
- **Technical Constraints**: [Platform limitations or opportunities]
- **Resource Availability**: [Team capacity and skills]
- **Market Trends**: [Industry shifts or emerging technologies]
