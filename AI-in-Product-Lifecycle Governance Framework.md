## Purpose

This framework establishes governance controls for AI-assisted product development. AI accelerates output; human judgment controls direction. Every feature, decision, and code change traces back to documented rationale and explicit approval.

This is a first draft talking point document for the team, not the Standard Operating Procedures (SOPs).  Explore, revise, and adapt these steps into the agentic workflow where possible.  

**The goal:** Use agents to track changes, document decisions, build logs, validate steps, ask for approval. 

**The core principle:** AI is a tool that can act as a person, but It's still just an engine that produces drafts, plans, and analysis. Humans evaluate, approve, and own outcomes. While our local token cost increases, you gain complete traceability. When someone asks "why did we build this feature?", you can answer with documented evidence: who requested it, who approved it, what problem it solved, and what alternatives were rejected.

---
#Model
## Governance Model

### Decision Authority Matrix

| Decision Type | AI Role | Human Role | Approval Required |
|--------------|---------|------------|-------------------|
| Feature ideation | Generate options, analyze competitors, surface gaps | Evaluate fit, reject/accept | PM sign-off |
| Requirements definition | Draft PRD sections, identify edge cases | Validate accuracy, set priorities | PM + Tech Lead |
| Architecture decisions | Propose patterns, analyze tradeoffs | Select approach, own risk | Tech Lead + Architect |
| Implementation | Write code, tests, documentation | Review, approve PRs | Code owner + peer |
| Security/compliance | Flag risks, generate checklists | Validate controls, accept residual risk | Security Lead |
| Release | Generate release notes, runbooks | Authorize deployment | Release Manager |

### Approval Chain Documentation

Every AI-assisted output requires:

1. **Request record**: What was asked, who asked, timestamp
2. **Source attribution**: What information the AI used to generate output
3. **Draft output**: The AI's response before human editing
4. **Human modifications**: What changed and why
5. **Approval record**: Who approved, timestamp, any conditions
6. **Rationale capture**: Why this approach over alternatives

This creates an audit trail. Six months later, you can reconstruct the decision context.

---
#Phases
## Lifecycle Phases

#Phase-Discovery
### Phase 1: Discovery and Ideation

**Objective**: Generate and evaluate feature candidates with full documentation.

**AI Activities**:
- Analyze market data, competitor features, user feedback
- Generate feature concepts with problem statements
- Draft opportunity assessments (reach, impact, confidence, effort)
- Identify potential risks and dependencies

**Human Activities**:
- Review AI-generated analysis for accuracy
- Add context AI cannot access (strategy, politics, constraints)
- Select candidates for further exploration
- Reject and document why others don't proceed

**Required Outputs**:

| Output | Owner | Approval |
|--------|-------|----------|
| Feature Candidate Brief | PM | PM Director |
| Opportunity Score | PM + AI | PM Director |
| Initial Risk Assessment | PM | PM Director |
| Decision Record (proceed/kill) | PM | PM Director |

**Feature Candidate Brief Template**:

```markdown
## Feature: [Name]

### Problem Statement
[AI drafts, human validates]

### Proposed Solution
[AI drafts, human validates]

### Target Users
[AI identifies from data, human confirms]

### Success Metrics
[AI proposes, human selects]

### Initial Risk Flags
[AI generates, human validates]

### Source Attribution
- Data sources used: [list]
- Competitor analysis date: [date]
- User feedback period: [range]

### Approval
- Drafted by: [name] using [AI model]
- Reviewed by: [name]
- Approved to proceed: [name], [date]
- Decision rationale: [why this over alternatives]
```

---
#Phase-Requirements
### Phase 2: Requirements Definition

**Objective**: Produce complete, validated requirements with change tracking.

**AI Activities**:
- Draft PRD sections from approved Feature Candidate Brief
- Generate user stories with acceptance criteria
- Identify edge cases and error states
- Propose technical constraints and dependencies
- Draft security and compliance requirements

**Human Activities**:
- Validate requirements against actual user needs
- Prioritize requirements (must/should/could/won't)
- Resolve ambiguities AI cannot clarify
- Approve final PRD

**Required Outputs**:

| Output | Owner | Approval |
|--------|-------|----------|
| Product Requirements Document | PM | PM Director + Tech Lead |
| User Story Set | PM | PM + QA Lead |
| Technical Constraints | Tech Lead | Architect |
| Security Requirements | Security Lead | CISO |
| Dependency Map | Tech Lead | Architect |

**PRD Change Log Entry Format**:

```markdown
## Change [ID]: [Title]
- Date: [timestamp]
- Requestor: [name]
- Section Modified: [PRD section]
- Previous Content: [quote]
- New Content: [quote]
- Rationale: [why change needed]
- AI Assistance: [what AI drafted vs human added]
- Approved by: [name], [timestamp]
```

Every PRD modification gets logged. No silent edits.

---
#Phase-Architecture
### Phase 3: Architecture and Design

**Objective**: Produce technical designs with explicit tradeoff documentation.

**AI Activities**:
- Generate architecture options based on requirements
- Analyze tradeoffs (performance, cost, complexity, risk)
- Draft technical design documents
- Identify integration points and failure modes
- Generate security threat models

**Human Activities**:
- Evaluate architecture options against constraints
- Select approach and document decision rationale
- Validate threat models against actual risk tolerance
- Approve design for implementation

**Required Outputs**:

| Output | Owner | Approval |
|--------|-------|----------|
| Architecture Decision Record (ADR) | Tech Lead | Architect + Security |
| Technical Design Document | Tech Lead | Architect |
| Threat Model | Security Lead | Security Lead + Tech Lead |
| Capacity Plan | Tech Lead | Operations |
| Integration Plan | Tech Lead | Dependent team leads |

**Architecture Decision Record Template**:

```markdown
## ADR-[Number]: [Title]

### Status
[Proposed | Accepted | Deprecated | Superseded]

### Context
[AI generates from requirements, human validates]

### Options Considered

#### Option A: [Name]
- Description: [AI drafts]
- Pros: [AI identifies]
- Cons: [AI identifies]
- Estimated effort: [AI estimates, human validates]

#### Option B: [Name]
[Same structure]

### Decision
[Human selects]

### Rationale
[Human writes: why this option over others]

### Consequences
[AI identifies, human validates]

### AI Contribution
- Options generated by: [model, date]
- Analysis reviewed by: [name]
- Human additions: [what wasn't AI-generated]

### Approval
- Proposed by: [name]
- Approved by: [name], [date]
```

---
#Phase-Planning 
### Phase 4: Implementation Planning

**Objective**: Create execution plan before any code is written.

**AI Activities**:
- Break features into implementation tasks
- Estimate effort based on similar past work
- Generate implementation sequence
- Draft code structure and patterns
- Identify testing requirements
- Generate dependency setup documentation

**Human Activities**:
- Validate task breakdown completeness
- Adjust estimates based on team knowledge
- Approve implementation sequence
- Assign owners to tasks

**Required Outputs**:

| Output | Owner | Approval |
|--------|-------|----------|
| Implementation Plan | Tech Lead | Tech Lead + PM |
| Task Breakdown | Tech Lead | Tech Lead |
| Dependency Setup Guide | Tech Lead | Operations |
| Testing Strategy | QA Lead | QA Lead + Tech Lead |
| Rollback Plan | Tech Lead | Operations |

**Pre-Implementation Checklist** (must be complete before coding starts):

- [ ] PRD approved and locked
- [ ] Architecture decision recorded
- [ ] Security review complete
- [ ] Dependencies documented
- [ ] Testing strategy approved
- [ ] Rollback plan exists
- [ ] Implementation tasks assigned
- [ ] Success criteria defined
- [ ] All approvals logged in process log

---
#Phase-Development
### Phase 5: Development

**Objective**: Produce code with full documentation of AI assistance.

**AI Activities**:
- Generate code drafts based on approved design
- Write unit tests
- Draft documentation
- Identify potential bugs and security issues
- Generate code review checklists

**Human Activities**:
- Review all AI-generated code
- Validate against requirements
- Ensure security controls implemented
- Approve pull requests
- Document any deviations from plan

**Required Outputs**:

| Output | Owner | Approval |
|--------|-------|----------|
| Code (with AI attribution) | Developer | Code owner + peer reviewer |
| Unit Tests | Developer | QA Lead |
| Code Documentation | Developer | Tech Lead |
| Security Scan Results | Security tools | Security Lead |
| PR Approval Record | Reviewer | Code owner |

**AI Code Attribution Standard**:

Every file with AI-generated code includes a header comment:

```
/**
 * AI Assistance Log
 * -----------------
 * Generated: [date]
 * Model: [model name/version]
 * Prompt summary: [what was requested]
 * Human modifications:
 *   - [list significant changes]
 * Reviewed by: [name], [date]
 * Approved by: [name], [date]
 * PRD Reference: [document name/date or revision]
 */
```

This isn't bureaucracy. It's traceability. When a bug appears in AI-generated code two years later, you know the generation context.

**Pull Request Template with AI Disclosure**:

```markdown
## Summary
[What this PR does]

## AI Assistance
- AI-generated code: [yes/no, percentage estimate]
- Model used: [name]
- Files with AI contribution: [list]
- Human review: [what was validated]

## Testing
- Unit tests: [pass/fail]
- Integration tests: [pass/fail]
- Manual testing: [completed by, date]

## Security
- Security scan: [pass/fail]
- Vulnerabilities addressed: [list or N/A]

## Checklist
- [ ] Code follows style guide
- [ ] Tests pass
- [ ] Documentation updated
- [ ] No secrets in code
- [ ] AI attribution comments added

## Approval
- Reviewed by: [name]
- Approved by: [code owner]
```

---
#Phase-QA
### Phase 6: Quality Assurance

**Objective**: Validate implementation meets requirements with documented test coverage.

**AI Activities**:
- Generate test cases from requirements
- Draft test scripts
- Analyze test results for patterns
- Identify untested edge cases
- Generate bug reports from test failures

**Human Activities**:
- Validate test coverage against requirements
- Execute exploratory testing
- Prioritize bugs
- Approve quality gate passage

**Required Outputs**:

| Output | Owner | Approval |
|--------|-------|----------|
| Test Plan | QA Lead | QA Lead + PM |
| Test Results | QA Engineer | QA Lead |
| Bug Reports | QA Engineer | Tech Lead for priority |
| Coverage Report | QA Lead | Tech Lead |
| Quality Gate Sign-off | QA Lead | QA Lead + Tech Lead |

---
#Phase-Security
### Phase 7: Security Review

**Objective**: Validate security controls before release.

**AI Activities**:
- Run automated security scans
- Generate vulnerability reports
- Draft remediation recommendations
- Update threat model with findings

**Human Activities**:
- Validate scan results (false positives)
- Assess actual risk of findings
- Approve remediation approach
- Accept residual risk with documentation

**Required Outputs**:

| Output | Owner | Approval |
|--------|-------|----------|
| Security Scan Report | Security tools | Security Lead |
| Vulnerability Assessment | Security Lead | Security Lead |
| Remediation Plan | Security Lead + Tech Lead | Security Lead |
| Risk Acceptance (if any) | Security Lead | CISO |
| Security Sign-off | Security Lead | Security Lead |

---
#Phase-Release
### Phase 8: Release

**Objective**: Deploy with full documentation and rollback capability.

**AI Activities**:
- Generate release notes from changelog
- Draft runbook procedures
- Create rollback scripts
- Generate monitoring dashboards

**Human Activities**:
- Validate release notes accuracy
- Approve deployment plan
- Execute deployment
- Monitor post-release

**Required Outputs**:

| Output | Owner | Approval |
|--------|-------|----------|
| Release Notes | PM | PM |
| Deployment Runbook | Operations | Operations Lead |
| Rollback Procedure | Operations | Operations Lead + Tech Lead |
| Monitoring Config | Operations | Operations Lead |
| Release Approval | Release Manager | Release Manager |

---
#Documents
## Document System

### Core Documents

These documents are required for every feature:

1. **Feature Candidate Brief**: Initial feature proposal with problem statement and success criteria
2. **Product Requirements Document (PRD)**: Complete requirements with acceptance criteria
3. **Architecture Decision Record (ADR)**: Technical approach with alternatives considered
4. **Implementation Plan**: Task breakdown with estimates and owners
5. **Test Plan**: Testing approach with coverage targets
6. **Security Assessment**: Threat model and security controls
7. **Release Package**: Release notes, runbook, rollback plan

### Process Logs

Two logs track all activity:

**Feature Changelog**: Records every modification to feature requirements, design, or implementation. Entries include timestamp, author, change description, rationale, and approval.

```markdown
## Changelog: [Feature Name]

### [Date] - [Change ID]
- Author: [name]
- Type: [requirement | design | implementation | security]
- Change: [description]
- Rationale: [why]
- AI contribution: [what AI drafted]
- Approved by: [name]

### [Date] - [Change ID]
[...]
```

**Process Approval Log**: Records every approval decision. This is your audit trail for governance.

```markdown
## Approval Log: [Feature Name]

### [Date] - [Approval ID]
- Phase: [discovery | requirements | design | implementation | QA | security | release]
- Decision: [approved | rejected | conditional]
- Approver: [name, role]
- Conditions: [any requirements for approval, or N/A]
- Documentation reviewed: [list of documents]
- Notes: [additional context]

### [Date] - [Approval ID]
[...]
```

---

## Role-Specific Guides

#Role-PM
### Guide for Product Managers

**Your role**: Own the "what" and "why". AI drafts; you validate, refine, and approve.

**Daily workflow**:

1. **Morning review**: Check AI-generated analysis from overnight. Validate accuracy. Flag errors.
2. **Drafting sessions**: Use AI to draft PRD sections, user stories, success metrics. Review every output before sharing.
3. **Stakeholder communication**: AI can draft updates, but you own the message. Review for accuracy and tone.
4. **Decision documentation**: When you make a decision, document rationale. AI can help structure the record.

**What AI does well for you**:
- Draft PRD sections from rough notes
- Generate user stories with acceptance criteria
- Analyze competitor features
- Identify edge cases you might miss
- Create structured documentation from unstructured input

**What AI cannot do for you**:
- Understand organizational politics
- Know undocumented strategy constraints
- Validate requirements against actual user conversations
- Make priority tradeoffs
- Take accountability for decisions

**Required documentation**:
- Approve all Feature Candidate Briefs before engineering work
- Sign off on PRD before implementation planning
- Document rationale for priority decisions
- Log all requirement changes in feature changelog

**Approval authorities**:
- Feature candidates (approve with PM Director)
- Requirements (approve with Tech Lead)
- Release notes (sole approval)

---
#Role-EngineeringLead
### Guide for Engineering Leaders

**Your role**: Own the "how". AI generates options and drafts; you evaluate, select, and approve.

**Daily workflow**:

1. **Architecture reviews**: Use AI to generate options. Evaluate against real constraints. Document selection rationale.
2. **Implementation oversight**: Review AI-generated task breakdowns. Validate estimates based on team capability.
3. **Code review**: Check AI attribution on PRs. Verify human review was substantive, not rubber-stamp.
4. **Technical debt tracking**: Use AI to identify patterns. Prioritize based on actual impact.

**What AI does well for you**:
- Generate architecture options with tradeoff analysis
- Draft technical design documents
- Estimate effort based on similar past work
- Identify integration risks
- Generate code review checklists

**What AI cannot do for you**:
- Know your team's actual velocity
- Understand tribal knowledge about your codebase
- Navigate relationships with dependent teams
- Make risk/speed tradeoffs for your context
- Take accountability for technical decisions

**Required documentation**:
- Architecture Decision Records for all significant choices
- Implementation plans before coding starts
- PR approval with AI attribution review
- Technical debt logged with priority rationale

**Approval authorities**:
- Architecture decisions (approve with Architect)
- Implementation plans (approve with PM)
- Pull requests (code owner authority)
- Technical debt prioritization (sole approval)

---
#Role-Developer
### Guide for Developers

**Your role**: Produce code with full AI attribution and human validation.

**Daily workflow**:

1. **Task pickup**: Review approved implementation plan. Understand requirements before asking AI to generate code.
2. **AI-assisted coding**: Generate code drafts. Review every line. Don't commit AI output without understanding it.
3. **Documentation**: AI can draft; you validate. Include AI attribution headers.
4. **Testing**: AI generates test cases. You validate coverage. Add edge cases AI missed.

**What AI does well for you**:
- Generate boilerplate code
- Draft unit tests
- Explain unfamiliar code patterns
- Identify potential bugs
- Generate documentation from code

**What AI cannot do for you**:
- Understand the full context of your codebase
- Know about undocumented requirements
- Guarantee generated code is secure
- Take responsibility for bugs in AI-generated code
- Review its own output critically

**Required documentation**:
- AI attribution comments in generated code
- PR descriptions with AI disclosure
- Test coverage documentation
- Any deviation from approved implementation plan

**Approval requirements**:
- All PRs require code owner + peer review
- AI-generated code requires explicit disclosure
- Security-sensitive changes require security review

**Non-negotiable rules**:
1. Never commit AI-generated code without reading and understanding it
2. Always disclose AI assistance in PRs
3. Always add AI attribution headers to generated files
4. Test AI-generated code as thoroughly as human-written code
5. If AI generates something you don't understand, learn it or don't use it

---
#Role-QA
### Guide for QA Engineers

**Your role**: Validate that implementation meets requirements. AI generates test cases; you ensure coverage.

**Daily workflow**:

1. **Test planning**: Review PRD. Use AI to generate test cases. Add cases AI missed based on domain knowledge.
2. **Test execution**: Run automated tests. Perform exploratory testing AI cannot do.
3. **Bug documentation**: AI can help structure bug reports. You provide accurate reproduction steps.
4. **Coverage analysis**: Use AI to identify gaps. Validate against actual risk areas.

**What AI does well for you**:
- Generate test cases from requirements
- Draft test scripts
- Analyze test results for patterns
- Identify untested scenarios
- Structure bug reports

**What AI cannot do for you**:
- Perform exploratory testing with human intuition
- Understand user workflows from real experience
- Validate usability and user experience
- Make quality vs. schedule tradeoffs
- Accept risk on your behalf

**Required documentation**:
- Test plans with coverage targets
- Test results with pass/fail records
- Bug reports with clear reproduction steps
- Quality gate sign-off documentation

---
#Role-Security
### Guide for Security Engineers

**Your role**: Validate security controls and accept or reject risk. AI identifies issues; you assess actual risk.  You look for known or hidden issues and use the tools to confirm, validate, and assess.

**Daily workflow**:

1. **Threat modeling**: Use AI to draft threat models. Validate against your knowledge of actual attack patterns.
2. **Scan review**: AI runs scans. You validate findings (many are false positives). Prioritize real risks.
3. **Remediation guidance**: AI suggests fixes. You validate they actually address the vulnerability.
4. **Risk acceptance**: You document residual risk. AI cannot accept risk on behalf of the organization.

**What AI does well for you**:
- Run automated security scans
- Draft threat models
- Generate remediation recommendations
- Identify common vulnerability patterns
- Structure security documentation

**What AI cannot do for you**:
- Assess actual exploitability in your environment
- Understand your organization's risk tolerance
- Know about compensating controls not in code
- Accept risk on behalf of the organization
- Validate that fixes actually work

**Required documentation**:
- Threat models for each feature
- Vulnerability assessments with actual risk ratings
- Remediation plans with timelines
- Risk acceptance documentation (when applicable)
- Security sign-off for release

---
#Documents-Support
## Supporting Documents and Services

### Required Documents to Create

| Document | Purpose | Owner |
|----------|---------|-------|
| AI Acceptable Use Policy | Define permitted AI tools, use cases, restrictions | Security + Legal |
| AI Tool Configuration Guide | Standard prompts, model selection, output validation | Tech Lead |
| Document Templates Package | All templates from this framework, ready to use | PM |
| Approval Workflow Diagram | Visual representation of approval chains | PM |
| Training Curriculum | Role-based training for all team members | PM + Engineering Lead |
| Audit Procedure | How to audit compliance with this framework | Security |
| Exception Request Process | How to request deviations from standard process | PM Director |
| Metrics and Reporting Guide | What to measure, how to report | PM |

### Required Services and Tools

| Service | Purpose | Selection Criteria |
|---------|---------|-------------------|
| Document Management | Store and version all governance documents | Version control, access control, audit log |
| Approval Workflow Tool | Route approvals, capture decisions | Integration with docs, notification, audit trail |
| AI Usage Logging | Track all AI interactions for audit | Capture prompts, outputs, users, timestamps |
| Code Repository | Store code with AI attribution | Branch protection, PR templates, audit log |
| Security Scanning | Automated vulnerability detection | Integration with CI/CD, actionable findings |
| Test Management | Track test cases and results | Traceability to requirements, coverage reports |
| Change Management | Track changes across all artifacts | Cross-artifact traceability, impact analysis |

### Integration Requirements

The document management, approval workflow, and AI usage logging must integrate to provide:

1. **Full traceability**: From feature request through release, every decision links to documentation
2. **Audit capability**: Auditors can reconstruct the complete history of any feature
3. **Attribution tracking**: All AI contributions are logged and traceable
4. **Approval verification**: No artifact advances without required approvals

---
#Documents-Metrics
## Metrics and Compliance

### Process Compliance Metrics

Track these to ensure the framework is followed:

| Metric | Target | Measurement |
|--------|--------|-------------|
| Documentation completion | 100% of required docs for each feature | Checklist audit |
| Approval capture rate | 100% of approvals logged | Approval log audit |
| AI attribution compliance | 100% of AI-assisted code attributed | PR audit |
| Change log completeness | All changes documented | Change log review |

### Process Health Metrics

Track these to assess framework effectiveness:

| Metric | Purpose | Target |
|--------|---------|--------|
| Cycle time by phase | Identify bottlenecks | Baseline + improvement |
| Rework rate | Quality of AI outputs | Decreasing trend |
| Approval turnaround | Process efficiency | < 24 hours for standard approvals |
| Post-release defects | Output quality | Decreasing trend |

### Audit Schedule

| Audit Type | Frequency | Auditor |
|------------|-----------|---------|
| Document completeness | Per feature release | PM |
| AI attribution compliance | Weekly sample | Tech Lead |
| Approval log integrity | Monthly | Security |
| Full process audit | Quarterly | Internal Audit |

---
#Documents-Implementation
## Implementation Roadmap

### Phase 1: Foundation (Weeks 1-4)

- [ ] Publish AI Acceptable Use Policy
- [ ] Deploy document templates
- [ ] Configure approval workflow tool
- [ ] Train PMs and Tech Leads
- [ ] Select pilot feature

### Phase 2: Pilot (Weeks 5-8)

- [ ] Execute full framework on pilot feature
- [ ] Collect friction points and improvement suggestions
- [ ] Refine templates and processes
- [ ] Document lessons learned

### Phase 3: Rollout (Weeks 9-12)

- [ ] Train all engineering teams
- [ ] Deploy AI usage logging
- [ ] Begin enforcement on all new features
- [ ] Establish audit procedures

### Phase 4: Optimization (Ongoing)

- [ ] Monthly process review
- [ ] Quarterly framework updates
- [ ] Annual comprehensive audit
- [ ] Continuous template improvement

---
#Summary
## Why This Matters

The alternative is what most teams do now: AI generates output, humans accept or reject, and nobody documents why. Six months later, you cannot explain why a feature exists, why an architecture was chosen, or whether AI-generated code was properly reviewed.

This framework burns more tokens. It requires more documentation. It slows the immediate output speed.

But it gives you:

1. **Complete audit trail**: Every decision traced to a person, a rationale, and an approval
2. **AI transparency**: No black-box AI contributions. Every AI assist is logged and attributed
3. **Human accountability**: AI drafts; humans own. Clear responsibility for every outcome
4. **Defensible process**: When regulators, auditors, or executives ask "how did this happen?", you can show them
5. **Institutional memory**: New team members can understand why things are the way they are

AI does the typing. Humans do the thinking and deciding. The documentation proves it.

---
#Appendix
## Appendix A: Template Index

All templates referenced in this document:

1. Feature Candidate Brief Template (Phase 1)
2. PRD Change Log Entry Format (Phase 2)
3. Architecture Decision Record Template (Phase 3)
4. Pre-Implementation Checklist (Phase 4)
5. AI Code Attribution Standard (Phase 5)
6. Pull Request Template with AI Disclosure (Phase 5)
7. Feature Changelog Format (Document System)
8. Process Approval Log Format (Document System)

---

## Appendix B: Glossary

| Term | Definition |
|------|------------|
| ADR | Architecture Decision Record. Documents a technical decision with context, options considered, and rationale. |
| AI Attribution | Documentation of what AI contributed to an output, what model was used, and what human review occurred. |
| Approval Chain | The sequence of human approvals required before an artifact can advance to the next phase. |
| Feature Changelog | Running log of all changes to a feature's requirements, design, or implementation. |
| Process Approval Log | Running log of all approval decisions across all phases for a feature. |
| PRD | Product Requirements Document. Complete specification of what a feature does and how success is measured. |
| Traceability | The ability to track an artifact back to its origin, through all modifications, to its current state. |

---

*Document version: 1.2*
