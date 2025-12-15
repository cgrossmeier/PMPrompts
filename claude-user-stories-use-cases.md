# User Stories & Use Cases Development

**Platform:** Claude (Sonnet 4.5 / Opus 4)

---

## Prompt

I need your help developing comprehensive user stories and use cases that clearly connect product features to real customer needs. Act as an expert product manager who excels at translating customer problems into well-structured user stories that guide development teams while ensuring every feature delivers genuine customer value.

**Product Context:**
- Product name: [Your product]
- Product description: [What it does]
- Target users: [Primary personas]
- Stage: [Early concept / Active development / Enhancement]
- Development methodology: [Agile / Scrum / Other]

**Feature to Document:**
- Feature name: [What you're building]
- High-level purpose: [Why this exists]
- Known customer pain points: [Problems this addresses]

## User Story Framework

For each feature, help me create comprehensive documentation that includes:

### 1. Customer Context & Problem Statement

**Who experiences this problem:**
- Specific user persona(s)
- Job titles and responsibilities
- Technical skill level
- Organizational context

**The problem they face:**
- Current workflow or situation
- Specific pain points or friction
- Frequency and impact of the problem
- What they've tried that hasn't worked
- Cost of not solving this (time, money, frustration)

**Evidence this problem exists:**
- Customer interview quotes
- Support ticket themes
- Usage data showing the pain
- Sales feedback or lost deals
- Competitive intelligence

### 2. User Story (Standard Format)

**As a** [specific user persona]  
**I want** [specific capability or action]  
**So that** [business value or outcome achieved]

**Additional Context:**
- **Given** [initial context or preconditions]
- **When** [action or trigger]
- **Then** [expected outcome or result]

### 3. Detailed Use Cases

For this feature, describe 2-4 specific use cases:

**Use Case #1: [Primary/Happy Path]**

**Actor:** [Who is using this]

**Preconditions:**
- [What must be true before this use case]
- [User permissions or access required]
- [Data or setup that must exist]

**Trigger:** [What initiates this workflow]

**Main Flow:**
1. User [specific action]
2. System [response or processing]
3. User [next action]
4. System [outcome]
5. [Continue step-by-step through completion]

**Success Outcome:**
- [What the user accomplishes]
- [How they know they succeeded]
- [Value delivered]

**Alternative Flows:**
- **If** [alternate condition], **then** [different path]
- **If** [error condition], **then** [error handling]

**Edge Cases:**
- [Unusual but valid scenarios]
- [System behavior in edge conditions]

### 4. Acceptance Criteria

Clear, testable criteria that define "done":

**Functional Criteria:**
- [ ] User can [specific action] when [condition]
- [ ] System displays [expected output] after [action]
- [ ] User receives [feedback] when [event]
- [ ] Feature handles [edge case] by [behavior]

**Non-Functional Criteria:**
- [ ] Feature responds within [X seconds]
- [ ] Works on [browsers/devices]
- [ ] Accessible via [keyboard/screen reader]
- [ ] Handles [X] concurrent users
- [ ] Data persists/syncs within [timeframe]

**User Experience Criteria:**
- [ ] User can complete task without training/help
- [ ] Error messages are clear and actionable
- [ ] Feature integrates seamlessly with [existing workflow]
- [ ] Visual design matches [design system]

### 5. Jobs to Be Done Analysis

**Functional Job:**
What task is the customer trying to accomplish?

**Emotional Job:**
How does the customer want to feel while doing this?

**Social Job:**
How does this affect how others perceive the user?

**Job Success Metrics:**
How does the customer measure whether the job is done well?

### 6. Customer Value Proposition

**Value Delivered:**
- Time saved: [quantify if possible]
- Efficiency gained: [specific improvements]
- Errors prevented: [risk reduction]
- New capabilities enabled: [what's now possible]
- Experience improved: [quality of life benefits]

**Quantified Impact (if available):**
- Reduces [task] from [X time] to [Y time]
- Eliminates [X%] of [error type]
- Enables [X] new workflows
- Increases [metric] by [X%]

**Competitive Advantage:**
How does this compare to alternatives?
- Better than [competitor] because [reason]
- Unique in that [differentiation]
- Table stakes for [market segment]

### 7. User Personas Affected

For each persona who will use this feature:

**Primary Persona: [Name/Role]**
- **How they'll use it:** [Main use case]
- **Frequency:** [Daily/Weekly/Monthly/As-needed]
- **Importance:** [Critical/Important/Nice-to-have]
- **Skill level required:** [Novice/Intermediate/Expert]

**Secondary Persona: [Name/Role]**
- [Same structure as above]

### 8. Customer Journey Touchpoints

**Discovery:** How will users find this feature?

**Onboarding:** How will users learn to use it?

**Regular Use:** How does this fit into daily workflows?

**Advanced Usage:** What power-user capabilities exist?

**Support Needs:** When might users need help?

### 9. Success Metrics

**Usage Metrics:**
- Adoption rate: [Target %]
- Frequency of use: [Target uses per user per timeframe]
- Feature stickiness: [Return rate within X days]

**Outcome Metrics:**
- Task completion rate: [Target %]
- Time to complete task: [Target duration]
- Error rate: [Target %]
- User satisfaction: [Target score]

**Business Metrics:**
- Impact on conversion: [Expected change]
- Effect on retention: [Expected improvement]
- Revenue influence: [Direct or indirect impact]
- Support ticket reduction: [Expected decrease]

### 10. Feature Dependencies & Context

**Requires:**
- [Existing features this depends on]
- [Platform capabilities needed]
- [Data or integrations required]

**Enables:**
- [Future features this unlocks]
- [Workflows this supports]

**Related Features:**
- [Complementary capabilities]
- [User journey connections]

## Requested Output Format

Please provide a comprehensive user story document structured as:

### Executive Summary
- 2-3 sentence overview
- Primary customer value
- Strategic importance

### User Stories (Standard Format)
- 3-5 user stories covering main use cases
- Written in "As a / I want / So that" format

### Detailed Use Cases
- Step-by-step walkthrough of 2-4 scenarios
- Include happy path and key alternatives
- Cover edge cases and error handling

### Acceptance Criteria Checklist
- Testable criteria for functional requirements
- Non-functional requirements (performance, compatibility)
- UX quality criteria

### Jobs to Be Done Analysis
- Functional, emotional, and social jobs
- Success metrics from customer perspective

### Customer Value & Metrics
- Quantified value proposition
- Success metrics to track
- Business impact expectations

### Supporting Information
- Persona mapping
- Journey touchpoints
- Dependencies and context

## Story Writing Principles

When creating user stories, ensure they are:

**Customer-Centric:**
- Written from user perspective, not system perspective
- Focus on outcomes, not implementation
- Use customer language, not technical jargon

**Specific & Testable:**
- Clear enough that anyone can understand
- Specific enough to estimate and build
- Testable so we know when it's done

**Independent:**
- Can be developed separately from other stories
- Not overly dependent on specific implementation details
- Flexible enough for technical approach

**Valuable:**
- Delivers clear customer or business value
- Can explain "why" to any stakeholder
- Worth the effort to build and maintain

**Appropriately Sized:**
- Small enough to complete in a sprint
- Large enough to deliver meaningful value
- Can be split if too large

## Common Pitfalls to Avoid

**Don't write technical specifications:**
❌ "Add a button that calls the API endpoint"
✅ "User can save their work at any time so progress isn't lost"

**Don't skip the 'so that' (value):**
❌ "As a user, I want to filter the list"
✅ "As a user, I want to filter the list so I can quickly find relevant items"

**Don't make stories too vague:**
❌ "Improve the user experience"
✅ "Reduce steps to complete checkout from 5 to 3 so users complete purchases faster"

**Don't forget edge cases:**
- Include error handling in acceptance criteria
- Document what happens when things go wrong
- Define expected behavior for unusual inputs

**Don't lose sight of the customer:**
- Every feature should trace back to customer need
- If you can't explain customer value, reconsider the feature
- Use real customer quotes and scenarios

## Additional Context (Optional)

**Customer Research Available:**
- [Interview transcripts, survey data, usage analytics]

**Constraints:**
- [Technical limitations, timeline, resources]

**Success Examples:**
- [Similar features that worked well]

**Known Challenges:**
- [Anticipated difficulties or risks]

---

## Tips for Best Results

**Provide Real Customer Evidence:**
Include actual quotes, support tickets, or usage data that demonstrates the need

**Be Specific About Personas:**
The more detail about who the user is, the better the stories will be

**Quantify When Possible:**
Numbers make value concrete ("saves 2 hours per week" vs "saves time")

**Include Context:**
Explain where this fits in the broader product strategy and user journey

**Think End-to-End:**
Consider discovery, learning, regular use, and edge cases

**Collaborate:**
Share drafts with customers, designers, and engineers for feedback

**Iterate:**
Refine stories as you learn more during development

---

**Remember**: Great user stories connect every feature back to real customer needs. If you can't write a compelling user story with clear customer value, question whether the feature should be built at all. The best products are built when every line of code serves a documented customer need.
