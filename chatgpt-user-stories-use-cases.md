# User Stories & Use Cases Development

**Platform:** ChatGPT (GPT-4 / GPT-5)

---

## System Message

You are an expert product manager specializing in user story development and use case documentation. Your expertise includes:

- Writing clear, customer-centric user stories that connect features to real needs
- Developing comprehensive use cases that guide implementation
- Applying Jobs to Be Done framework to understand customer motivations
- Creating testable acceptance criteria
- Ensuring every feature traces back to documented customer value
- Translating customer research into actionable development requirements
- Balancing business goals with user needs

You help product teams ensure that every feature they build serves a genuine customer need with measurable value. Your user stories are specific, testable, and provide clear guidance for design and engineering teams.

---

## User Message

Help me develop comprehensive user stories and use cases that connect product features to customer needs.

### Product Context

**Product Information:**
- **Product Name:** [Your product]
- **Description:** [What it does and who it serves]
- **Target Users:** [Primary user personas]
- **Development Stage:** [Concept / Active Development / Enhancement]
- **Methodology:** [Agile / Scrum / Kanban / Other]

**Feature to Document:**
- **Feature Name:** [What you're building]
- **High-Level Purpose:** [Why this exists]
- **Customer Pain Points:** [Problems this addresses]
- **Strategic Importance:** [How this supports product/business goals]

**Available Research:**
- Customer interviews: [Summary or key quotes]
- Usage data: [Relevant analytics or patterns]
- Support tickets: [Common issues or requests]
- Competitive analysis: [How others solve this]

### Required Deliverables

Generate comprehensive user story documentation with the following structure:

#### 1. Customer Problem Statement

**Problem Context:**

| Element | Description |
|---------|-------------|
| **Who** | Specific user persona(s) experiencing this problem |
| **What** | The problem or pain point in detail |
| **Where** | Context where problem occurs (workflow, environment) |
| **When** | Frequency and timing of problem |
| **Why It Matters** | Impact and cost of not solving |
| **Current Workarounds** | How users cope today |

**Evidence:**
- Customer quote 1: "[Direct quote from research]"
- Customer quote 2: "[Direct quote from research]"
- Data point: [Usage statistics or support volume]
- Market context: [Competitive or industry trend]

#### 2. User Stories (Standard Format)

Create 3-5 user stories covering main scenarios:

**Primary User Story:**

```
As a [specific persona with context]
I want [specific capability]
So that [measurable outcome or business value]
```

**Given-When-Then Format:**

```
Given [initial context/preconditions]
When [user action or trigger]
Then [expected system response and outcome]
```

**Story Details:**

| Attribute | Value |
|-----------|-------|
| **Story ID** | [US-XXX] |
| **Priority** | Critical / High / Medium / Low |
| **Estimate** | [Story points or t-shirt size] |
| **Sprint Target** | [Which sprint or release] |
| **Dependencies** | [Other stories or capabilities needed] |

#### 3. Detailed Use Cases

For each major scenario, provide step-by-step use case:

**Use Case: [Name - e.g., "Happy Path: First-Time User"]**

| Element | Details |
|---------|---------|
| **UC ID** | UC-[XXX] |
| **Actor** | [User persona] |
| **Goal** | [What user wants to accomplish] |
| **Frequency** | Daily / Weekly / Monthly / As-needed |
| **Importance** | Critical / Important / Nice-to-have |

**Preconditions:**
- [ ] [Condition that must be true before starting]
- [ ] [Required permissions or access]
- [ ] [Data or setup that must exist]

**Trigger:** [What initiates this workflow]

**Main Success Scenario:**

| Step | Actor | Action | System Response |
|------|-------|--------|-----------------|
| 1 | User | [Specific action] | [System behavior] |
| 2 | System | [Processing] | [Result displayed] |
| 3 | User | [Next action] | [Feedback provided] |
| 4 | System | [Final processing] | [Completion state] |

**Success Outcome:**
- User accomplishes: [Specific goal achieved]
- Success indicator: [How user knows it worked]
- Value delivered: [Benefit realized]

**Alternative Flows:**

| Condition | Alternative Path | Outcome |
|-----------|-----------------|---------|
| If [alternate scenario] | [Steps taken instead] | [Result] |
| If [error condition] | [Error handling] | [Recovery or message] |

**Exception Flows:**

| Error | Cause | System Response | User Action |
|-------|-------|-----------------|-------------|
| [Error type] | [What went wrong] | [Error handling] | [How to recover] |

**Post-Conditions:**
- [ ] [System state after completion]
- [ ] [Data created or modified]
- [ ] [User state or permissions updated]

#### 4. Acceptance Criteria (Testable)

**Functional Requirements:**

- [ ] **Given** [context], **When** [action], **Then** [expected result]
- [ ] User can [specific action] and sees [specific feedback]
- [ ] System validates [input type] and shows [error message] for invalid input
- [ ] Feature correctly handles [edge case] by [behavior]
- [ ] Data is [created/updated/deleted] as expected when [action]

**Non-Functional Requirements:**

| Category | Requirement | Target | How to Test |
|----------|-------------|--------|-------------|
| Performance | Response time | < [X] seconds | [Test method] |
| Scalability | Concurrent users | [X] users | [Load test] |
| Compatibility | Browsers/devices | [List] | [Cross-browser test] |
| Accessibility | WCAG compliance | Level [AA/AAA] | [Accessibility audit] |
| Reliability | Uptime | [X]% | [Monitoring] |

**User Experience Requirements:**

- [ ] User can complete task without documentation or training
- [ ] Error messages are clear and suggest corrective action
- [ ] Feature integrates seamlessly with existing workflows
- [ ] Visual design follows [design system/guidelines]
- [ ] User receives confirmation for all state-changing actions

**Security & Privacy:**

- [ ] Only authorized users can access feature
- [ ] Sensitive data is [encrypted/masked/protected]
- [ ] Audit trail captures [relevant events]
- [ ] Complies with [GDPR/HIPAA/other regulations]

#### 5. Jobs to Be Done Analysis

**Functional Job:**
- **Job Statement:** When [situation], I want to [motivation], so I can [outcome]
- **Success Metrics:** [How customer measures if job is done well]

**Emotional Job:**
- **Desired Feeling:** Customer wants to feel [emotion]
- **Avoided Feeling:** Customer wants to avoid feeling [emotion]

**Social Job:**
- **Perception Goal:** How user wants others to perceive them
- **Social Context:** How this affects user's role or reputation

**Job Metrics:**

| Dimension | Current State | Desired State | Gap |
|-----------|---------------|---------------|-----|
| Speed | [Current time] | [Target time] | [Improvement needed] |
| Output | [Current result] | [Desired result] | [Quality gap] |
| Cost | [Current cost] | [Target cost] | [Savings opportunity] |

#### 6. Customer Value Proposition

**Value Delivered:**

| Value Type | Specific Benefit | Quantified Impact |
|------------|------------------|-------------------|
| Time Savings | [Specific task] | From [X] to [Y] minutes |
| Efficiency | [Process improvement] | [X]% reduction in steps |
| Error Reduction | [Error prevented] | [X]% fewer mistakes |
| New Capability | [What's now possible] | [Business impact] |
| Experience | [Quality improvement] | [Satisfaction score] |

**Before vs After:**

| Aspect | Before (Current State) | After (With Feature) | Improvement |
|--------|------------------------|----------------------|-------------|
| Time to complete | [X minutes] | [Y minutes] | [Z]% faster |
| Steps required | [X steps] | [Y steps] | [Z] fewer |
| Error rate | [X]% | [Y]% | [Z]% reduction |
| User satisfaction | [Score] | [Target] | [Improvement] |

**Competitive Comparison:**

| Capability | Our Solution | Competitor A | Competitor B | Advantage |
|------------|-------------|--------------|--------------|-----------|
| [Feature aspect] | [Our approach] | [Their approach] | [Their approach] | [Why ours is better] |

#### 7. User Persona Mapping

**Primary Persona: [Name/Role]**

| Attribute | Details |
|-----------|---------|
| **Who** | [Job title, responsibility] |
| **Use Frequency** | Daily / Weekly / Monthly |
| **Importance** | Critical / Important / Nice-to-have |
| **Skill Level** | Novice / Intermediate / Expert |
| **Main Use Case** | [Primary way they'll use this] |
| **Success Criteria** | [How they'll measure value] |

**Secondary Persona: [Name/Role]**
[Same structure as above]

**Persona-Specific Considerations:**

| Persona | Special Needs | Potential Barriers | Support Required |
|---------|---------------|-------------------|------------------|
| [Persona 1] | [Specific requirement] | [Challenge to adoption] | [Help needed] |
| [Persona 2] | [Specific requirement] | [Challenge to adoption] | [Help needed] |

#### 8. Customer Journey Integration

**Journey Touchpoints:**

| Stage | User Action | Feature Role | Success Metric |
|-------|-------------|--------------|----------------|
| **Discovery** | How user finds feature | [Discoverability method] | [Adoption rate] |
| **First Use** | Initial experience | [Onboarding approach] | [Activation rate] |
| **Learning** | Skill development | [Education/help] | [Competency time] |
| **Regular Use** | Daily workflow | [Integration points] | [Usage frequency] |
| **Advanced** | Power user capabilities | [Advanced features] | [Feature depth] |
| **Support** | When help needed | [Support resources] | [Resolution time] |

**Workflow Integration:**

| Existing Workflow | Integration Point | User Benefit |
|------------------|-------------------|--------------|
| [Current process] | [How feature fits] | [Value added] |

#### 9. Success Metrics & Tracking

**Usage Metrics:**

| Metric | Target | Measurement Method | Review Cadence |
|--------|--------|-------------------|----------------|
| Adoption Rate | [X]% of target users | [Analytics tracking] | Weekly |
| Feature Usage | [X] uses per user per week | [Event tracking] | Daily |
| Retention | [X]% return within 7 days | [Cohort analysis] | Weekly |

**Outcome Metrics:**

| Metric | Baseline | Target | Timeline | Owner |
|--------|----------|--------|----------|-------|
| Task Completion Rate | [X]% | [Y]% | [Date] | [Team/Person] |
| Time to Complete | [X] min | [Y] min | [Date] | [Team/Person] |
| Error Rate | [X]% | [Y]% | [Date] | [Team/Person] |
| User Satisfaction (CSAT) | [X]/10 | [Y]/10 | [Date] | [Team/Person] |

**Business Impact Metrics:**

| Metric | Expected Impact | Measurement | Attribution Method |
|--------|----------------|-------------|-------------------|
| Conversion Rate | [+X]% | [Analytics] | [A/B test or cohort] |
| Customer Retention | [+X]% | [Churn analysis] | [Feature usage correlation] |
| Revenue | [$X] or [+X]% | [Financial tracking] | [Revenue attribution] |
| Support Tickets | [-X]% | [Ticket system] | [Topic analysis] |

#### 10. Dependencies & Related Work

**Technical Dependencies:**

| Dependency | Status | Owner | Risk if Delayed |
|------------|--------|-------|-----------------|
| [API/service/data] | Ready / In Progress / Blocked | [Team] | [Impact] |

**Feature Dependencies:**

| Related Feature | Relationship | Priority | Impact |
|----------------|--------------|----------|--------|
| [Feature name] | Required before / Enables / Complementary | [Priority] | [How affects this story] |

**Integration Points:**

| System/Feature | Integration Type | Complexity | Owner |
|---------------|------------------|------------|-------|
| [System name] | Data / API / UI / Workflow | High / Medium / Low | [Team] |

### Output Requirements

Please provide a comprehensive user story document formatted as follows:

**1. Executive Summary (1 paragraph)**
- Customer problem and value proposition
- Strategic importance
- Expected impact

**2. User Stories Collection**
- 3-5 stories in standard format
- Prioritized by importance
- Story point estimates

**3. Detailed Use Cases (2-4 scenarios)**
- Happy path
- Key alternative flows
- Error handling
- Complete step-by-step workflows

**4. Acceptance Criteria Checklist**
- Functional requirements (testable)
- Non-functional requirements (measurable)
- UX quality criteria
- Security/compliance requirements

**5. JTBD Analysis**
- Functional, emotional, social jobs
- Current vs desired state
- Success metrics

**6. Value Proposition**
- Quantified benefits
- Before/after comparison
- Competitive advantages

**7. Metrics Dashboard**
- Usage metrics to track
- Outcome metrics with targets
- Business impact expectations

**8. Supporting Information**
- Persona mapping
- Journey integration
- Dependencies and risks

### Quality Standards

Ensure all user stories meet these criteria:

**INVEST Principles:**
- **Independent:** Can be developed separately
- **Negotiable:** Flexible on implementation details
- **Valuable:** Clear customer or business value
- **Estimable:** Can be sized by development team
- **Small:** Fits within a sprint
- **Testable:** Has clear acceptance criteria

**Customer-Centric:**
- Written from user perspective
- Focuses on outcomes, not features
- Uses customer language
- Traces to real customer evidence

**Actionable:**
- Specific enough to design and build
- Clear enough for anyone to understand
- Testable so team knows when done
- Complete with context and criteria

### Examples for Reference

**Good User Story:**
```
As a sales manager reviewing team performance
I want to see individual rep metrics side-by-side
So that I can quickly identify coaching opportunities and top performers

Given I'm viewing the team dashboard
When I select "Compare Reps"
Then I see a sortable table with key metrics for each rep
```

**Poor User Story:**
```
As a user
I want better reports
So that I can see data
```
[Too vague, no specificity, unclear value]

---

Generate comprehensive user story documentation that ensures every feature we build delivers measurable customer value.
