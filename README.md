# Product Management & Leadership Prompts

**A comprehensive library of AI-optimized prompts for product management professionals**

> Accelerate strategic planning, market research, stakeholder communication, and product development with battle-tested prompts for Claude and ChatGPT.  Many of these prompts are here to either inform you or help you to generate a document.  In all cases, they are a starting point. Each prompt includes more data than any single organization will ever need, but enough context for anyone to remove what they do not need. Use these prompts, trim unnecessary content, and optimize your product management processes.
>


[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## 📚 What's Inside

This repository contains **60+ professional-grade prompts** specifically designed for product managers, product leaders, and strategic decision-makers. Each prompt is:

- ✅ **Platform-Optimized** - Separate versions for Claude (Sonnet 4.5/Opus 4) and ChatGPT (GPT-4/GPT-5)
- ✅ **Production-Ready** - Tested and refined for real-world PM workflows
- ✅ **Framework-Based** - Built on established PM methodologies (RICE, SWOT, Kano, MoSCoW, etc.)
- ✅ **Comprehensive** - Detailed analysis frameworks with actionable outputs
- ✅ **Customizable** - Easy to adapt to your specific product and context

---

## 🎯 Quick Start

### Choose Your Use Case

| I Need To... | Use This Prompt |
|--------------|-----------------|
| Understand customer pain points | Pain Points Analysis(#pain-points) (Claude / ChatGPT) |
| Analyze competitors | Competitor Analysis(#competitor-analysis) (Claude / ChatGPT) |
| Develop product strategy | SWOT Analysis(#swot-analysis) (Claude / ChatGPT) |
| Get executive buy-in | Concept PRD(#concept-prd) (Claude / ChatGPT) |
| Create board materials | One-Page Overview(#one-page-overview) (Claude / ChatGPT) |
| Decide build vs buy | Build vs Buy(#build-vs-buy) (Claude / ChatGPT) |
| Find partners | Potential Partners(#potential-partners) (Claude / ChatGPT) |
| Plan roadmap | Sample Roadmap(#sample-roadmap) (Claude / ChatGPT) |
| Generate enhancement ideas | 25 Enhancements(#enhancement-generation) (Multiple) |
| Prioritize features | Prioritization Frameworks(#prioritization) (Multiple) |

### Basic Usage

1. **Select Platform**: Choose Claude or ChatGPT prompt version; some are non-platform specific.
2. **Open Prompt**: Click the relevant `.md` file
3. **Fill Context**: Edit prompt and replace `[bracketed]` placeholders with your details where possible.  You can also advise your LLM to make assumptions for the rough draft.
4. **Copy & Run**: Paste into your AI platform
5. **Iterate**: Refine results with follow-up questions

### Example

```markdown
From: chatgpt-pain-points.md

Product: [Acme Analytics Platform]  → Product: "Enterprise data visualization tool."
Target Market: [Industry]           → Target Market: "Fortune 500 finance teams."
Known Issues: [List]                → Known Issues: "Slow dashboard loading, complex onboarding. RedFish API is incomplete."
```

---

## 📂 Repository Structure

### 🎨 Profile Prompts (2 prompts)

Customize AI behavior for your role:

| Prompt | Purpose |
|--------|---------|
| **profile-director-product-management.md** | Strategic, executive-level guidance for portfolio management |
| **profile-senior-ai-product-manager.md** | Hands-on execution focus for AI/ML products |

### 🔍 Market Research & Analysis (6 prompts)

Deep dive into markets, competitors, and strategic positioning:

| Topic | Claude | ChatGPT | Use For |
|-------|--------|---------|---------|
| **Pain Points** | `claude-pain-points.md` | `chatgpt-pain-points.md` | Customer problem identification and prioritization |
| **Competitor Analysis** | `claude-competitor-analysis.md` | `chatgpt-competitor-analysis.md` | Comprehensive competitive intelligence |
| **SWOT Analysis** | `claude-swot-analysis.md` | `chatgpt-swot-analysis.md` | Strategic strengths, weaknesses, opportunities, threats |

### 💼 Executive Communication (4 prompts)

Materials for leadership, boards, and stakeholders:

| Topic | Claude | ChatGPT | Use For |
|-------|--------|---------|---------|
| **Concept PRD** | `claude-concept-prd.md` | `chatgpt-concept-prd.md` | Executive approval documents |
| **One-Page Overview** | `claude-one-page-overview.md` | `chatgpt-one-page-overview.md` | Board/investor summaries |

### 🎯 Strategic Analysis (6 prompts)

High-level decisions and partnerships:

| Topic | Claude | ChatGPT | Use For |
|-------|--------|---------|---------|
| **Buy vs Build** | `claude-buy-vs-build.md` | `chatgpt-buy-vs-build.md` | Make-or-buy decisions |
| **Potential Partners** | `claude-potential-partners.md` | `chatgpt-potential-partners.md` | Partnership opportunity evaluation |
| **Trailing Leaders** | `claude-trailing-leaders.md` | `chatgpt-trailing-leaders.md` | Competitive gap analysis |

### 🗺️ Product Planning (4 prompts)

Roadmaps and storytelling:

| Topic | Claude | ChatGPT | Use For |
|-------|--------|---------|---------|
| **Sample Roadmap** | `claude-sample-roadmap.md` | `chatgpt-sample-roadmap.md` | Strategic roadmaps with dependencies |
| **Customer Adoption Arc** | `claude-customer-adoption-arc.md` | `chatgpt-customer-adoption-arc.md` | Success story narratives |

### 🚀 Enhancement Generation (10 prompts)

Generate 25 ideas for specific improvements:

| Focus Area | Claude | ChatGPT |
|------------|--------|---------|
| **Customer Adoption** | `claude-25-enhance-adoption.md` | `chatgpt-25-enhance-adoption.md` |
| **Usability** | `claude-25-enhance-usability.md` | `chatgpt-25-enhance-usability.md` |
| **Security** | `claude-25-enhance-security.md` | `chatgpt-25-enhance-security.md` |
| **Support Reduction** | `claude-25-reduce-tickets.md` | `chatgpt-25-reduce-tickets.md` |
| **Competitive Differentiation** | `claude-25-differentiate-competitor.md` | `chatgpt-25-differentiate-competitor.md` |

### 📊 Prioritization Frameworks (19 prompts)

Platform-agnostic frameworks for feature prioritization:

| Framework | Prompt File | Use Case |
|-----------|-------------|----------|
| **Financial Analysis** | `prompt-financial-analysis.md` | NPV, ROI, payback period analysis |
| **Value to Risk** | `prompt-value-to-risk-analysis.md` | Risk-adjusted prioritization |
| **Value to Cost** | `prompt-value-to-cost-analysis.md` | Efficiency-focused ranking |
| **RICE Scorecard** | `prompt-rice-scorecard.md` | Reach × Impact × Confidence / Effort |
| **Kano Model** | `prompt-kano-model.md` | Must-be, Performance, Delighter categorization |
| **Buy a Feature** | `prompt-buy-a-feature.md` | Customer budget allocation exercise |
| **MoSCoW** | `prompt-moscow-prioritization.md` | Must/Should/Could/Won't have |
| **Classification Ranking** | `prompt-classification-ranking.md` | Tier-based prioritization |
| **Stacked Ranking** | `prompt-stacked-ranking.md` | Forced ranking (#1 to #N) |
| **Feature Bucket** | `prompt-feature-bucket.md` | Strategic theme-based organization |

### 📋 Strategic Planning Prompts (7 prompts)

Comprehensive strategic frameworks:

| Topic | Prompt File |
|-------|-------------|
| **New Product Development** | `prompt-new-product-development.md` |
| **Competitive Analysis** | `prompt-competitive-analysis.md` |
| **Core Product Considerations** | `prompt-core-product-considerations.md` |
| **Product Release Structure** | `prompt-product-release-structure.md` |
| **Growth Planning** | `prompt-growth-planning.md` |
| **B2B Pricing Strategy** | `prompt-b2b-pricing-strategy.md` |
| **AI Implementation Strategy** | `prompt-ai-implementation-strategy.md` |

### 💡 Idea Generation (1 prompt)

| Topic | Prompt File |
|-------|-------------|
| **25 Enhancement Ideas** | `prompt-25-enhancement-ideas.md` |

---

## 🎓 Prompt Categories by PM Activity

### Discovery & Research
- Customer Pain Points Analysis
- Competitor Analysis
- SWOT Analysis
- Market Research
- Trailing Leaders Analysis

### Strategy & Planning
- New Product Development
- Core Product Considerations
- Growth Planning
- AI Implementation Strategy
- B2B Pricing Strategy

### Prioritization & Decision-Making
- Financial Analysis
- Value to Risk/Cost Analysis
- RICE, Kano, MoSCoW Frameworks
- Classification & Stacked Ranking
- Buy vs Build Analysis
- Feature Bucket Organization

### Communication & Stakeholders
- Concept PRD for Executives
- One-Page Product Overview
- Customer Adoption Story
- Sample Roadmap

### Execution & Enhancement
- 25 Enhancement Ideas (5 variations)
- Product Release Structure
- Potential Partners

---

## 💡 Platform Differences

### Claude Prompts (Sonnet 4.5 / Opus 4)
- **Structure**: Natural conversational flow with detailed frameworks
- **Strength**: Deep analytical thinking, comprehensive exploration
- **Best For**: Complex strategic analysis, nuanced decision-making
- **Style**: Step-by-step guidance, extensive context consideration

### ChatGPT Prompts (GPT-4 / GPT-5)
- **Structure**: System message + User message format
- **Strength**: Structured outputs, table-based deliverables
- **Best For**: Formatted reports, systematic analysis
- **Style**: Clear scoring rubrics, explicit output formats

---

## 🚀 Advanced Usage

### Chaining Prompts

For comprehensive projects, use prompts in sequence:

```
1. Pain Points Analysis → Understand problems
2. SWOT Analysis → Assess positioning  
3. Competitive Analysis → Map landscape
4. New Product Development → Define approach
5. Concept PRD → Get approval
6. Sample Roadmap → Plan execution
```

### Combining Frameworks

Use multiple prioritization methods together:

```
1. RICE Scorecard → Initial ranking
2. Value to Risk → Risk assessment
3. Kano Model → Customer satisfaction impact
4. Financial Analysis → Business case
→ Final decision with confidence
```

### Customization Tips

**Always Include:**
- Specific product context
- Target market details
- Current metrics/baseline
- Constraints and limitations
- Strategic objectives

**Enhance With:**
- Customer quotes
- Usage data
- Competitive intelligence
- Team capacity
- Budget parameters

---

## 📖 Detailed Use Cases

### For Product Managers
- Feature prioritization with multiple frameworks
- Customer research synthesis
- Competitive positioning
- Requirements documentation
- Stakeholder communication

### For Product Leaders
- Portfolio strategy development
- Executive presentations
- Board communications
- Resource allocation
- Team alignment

### For Founders & Executives
- Market opportunity assessment
- Strategic planning
- Investor communications
- Product vision articulation
- Go-to-market strategy

### For AI/ML Product Teams
- AI implementation planning
- Model selection strategy
- Responsible AI considerations
- Technical architecture decisions

---

## 🎯 Best Practices

### ✅ Do's

- **Provide Context**: Always fill in specific product details
- **Iterate**: Start broad, refine with follow-ups
- **Validate**: Cross-check AI outputs with real data
- **Combine**: Use multiple prompts for comprehensive analysis
- **Customize**: Adapt prompts to your terminology and process
- **Document**: Save successful variations for reuse

### ❌ Don'ts

- **Don't Skip Context**: Generic inputs get generic outputs
- **Don't Trust Blindly**: AI augments judgment, doesn't replace it
- **Don't Share Secrets**: Never include confidential information
- **Don't Use Once**: Iterate and refine for better results
- **Don't Ignore Domain Knowledge**: Your expertise is essential

---

## 🤝 Contributing

Contributions are welcome! If you have prompts that have worked well for you:

1. **Fork** the repository
2. **Add** your prompt following existing naming conventions:
   - `claude-[topic].md` for Claude prompts
   - `chatgpt-[topic].md` for ChatGPT prompts
   - `prompt-[framework].md` for platform-agnostic prompts
3. **Test** the prompt thoroughly
4. **Document** the use case and expected outputs
5. **Submit** a pull request

### Contribution Guidelines

- Clear, descriptive prompt names
- Comprehensive framework structure
- Include example placeholders
- Specify target AI platform
- Provide usage context
- Test with real scenarios

---

## 📝 Naming Conventions

```
claude-[topic].md           → Claude-optimized prompts
chatgpt-[topic].md          → ChatGPT-optimized prompts
prompt-[framework].md       → Platform-agnostic prompts
profile-[role].md           → Role-specific AI profiles
```

---

## 🔗 Related Resources

### Product Management Frameworks
- [RICE Prioritization](https://www.intercom.com/blog/rice-simple-prioritization-for-product-managers/)
- [Kano Model](https://www.productplan.com/glossary/kano-model/)
- [Jobs to Be Done](https://jtbd.info/)
- [MoSCoW Method](https://www.productplan.com/glossary/moscow-prioritization/)

### AI for Product Management
- [Anthropic Claude Documentation](https://docs.anthropic.com/)
- [OpenAI ChatGPT Documentation](https://platform.openai.com/docs/)
- [Prompt Engineering Guide](https://www.promptingguide.ai/)

---

## ⚠️ Important Considerations

### Privacy & Security
- **Never include** confidential customer data, proprietary information, or trade secrets
- **Mask sensitive details** when providing context
- **Use generic examples** rather than real company data
- **Review outputs** before sharing internally

### Limitations
- AI outputs are **starting points**, not final deliverables
- Requires **validation** with real customer research
- Context and **domain expertise remain essential**
- Results may need **significant customization**
- Not a replacement for **strategic thinking**

### Validation Required
- Cross-check competitive analysis with primary research
- Validate financial projections with actual data
- Test prioritization frameworks with stakeholders
- Confirm technical feasibility with engineering
- Verify market insights with customer interviews

---

## 📜 License

This repository is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

Built for the product management community. Special thanks to all contributors and the PM teams who've tested and refined these prompts in production environments.

---

## 📞 Support & Feedback

- **Issues**: Found a bug or have a suggestion? [Open an issue](https://github.com/cgrossmeier/PMPrompts/issues)
- **Discussions**: Questions or ideas? [Start a discussion](https://github.com/cgrossmeier/PMPrompts/discussions)
- **Pull Requests**: Want to contribute? [Submit a PR](https://github.com/cgrossmeier/PMPrompts/pulls)

---

## 🌟 Star History

If you find these prompts valuable, please consider starring the repository to help others discover it!

---

**Made with ❤️ for Product Managers** | Last Updated: December 2024
