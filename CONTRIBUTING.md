# Contributing to Product-Manager-LLM-Specific-Prompts

Thanks for helping improve this prompt library. This repository is a curated set of product leadership and product management prompts, plus supporting resources, examples, and role profiles. Contributions should make it easier for product teams to get consistent, high quality outputs from large language models (LLMs).

## Ways to contribute

You can contribute in several ways:

- Add a new prompt (ChatGPT, Claude, or model-agnostic).
- Improve an existing prompt (clarity, structure, better constraints, stronger output format).
- Add an example showing prompt input and output.
- Fix typos, broken links, or unclear instructions.
- Add or improve supporting resources (templates, rubrics, writing style guidance).

## Ground rules

- Do not include private, confidential, or personally identifying information (PII) in prompts or examples.
- Do not submit copyrighted text copied from paid sources, books, or articles.
- Keep prompts customer-centric and outcome-driven. Avoid fluff.
- Prefer deterministic structure. Ask the model for specific formats, tables, checklists, or JSON when useful.
- Treat medical, legal, and financial content carefully. Include disclaimers and escalation guidance where appropriate.
- Be respectful in all communication.

## Repository conventions

From the current file set, the repo uses a simple, flat structure and naming conventions. Follow these patterns unless a maintainer requests a change.

### File naming

Use kebab-case and a model prefix when relevant:

- `chatgpt-<topic>.md` for prompts tuned for ChatGPT.
- `claude-<topic>.md` for prompts tuned for Claude.
- `prompt-<topic>.md` for model-agnostic prompts.
- `profile-<role>.md` for role profiles.
- `__example<N>_<topic>_Prompt_and_Output.md` for complete examples.

Examples:
- `chatgpt-competitor-analysis.md`
- `claude-user-stories-use-cases.md`
- `prompt-ai-implementation-strategy.md`
- `profile-senior-ai-product-manager.md`


## Standard prompt format

New prompt files should follow this structure so others can scan, reuse, and adapt quickly.

### Template

Copy and paste this into your new prompt file and fill it in:

```md
# <Prompt Title>

## Purpose
One to two sentences describing what this prompt helps a product manager accomplish.

## Best for
- Primary user persona (example: PM, Director of Product, UX researcher)
- Primary situation (example: early discovery, roadmap planning, incident review)

## Inputs needed
List the common/minimum information a user should provide.

- Product context:
- Target users:
- Constraints:
- Output audience:
- Time horizon:

## Prompt
Paste the full prompt text below. Include role, goal, context, constraints, and output format.

```text
<Your prompt here>
```

## Output format
Describe the expected structure. Prefer a strict structure.

Example:
- Executive summary
- Assumptions
- Analysis
- Recommendations
- Risks and open questions

## Notes and guardrails
- Safety or compliance guidance (if relevant)
- Common failure modes and how to avoid them
- When not to use this prompt

## Example
Optional but strongly encouraged. Provide one realistic example input and a truncated example output.

### Prompt quality checklist

Before opening a pull request, confirm your prompt meets these checks:

- Clear role and goal.
- Explicit inputs and assumptions.
- Constraints are stated (time, scope, format, audience).
- Output format is unambiguous.
- Includes edge cases, risks, and validation steps when relevant.
- Uses customer language and ties work back to measurable value.
- Avoids sensitive data and disallowed content.

## Adding examples

Examples are often the highest leverage contribution because they show how the prompt behaves in practice.

When adding an example file:

- Use the `__example<N>_...` naming pattern.
- Include the exact prompt used.
- Include the exact inputs used (redact sensitive data).
- Include the output, but keep it reasonably sized.
- Add a short note describing what to look for (what makes the output good or bad).

## Updating existing prompts

If you update an existing prompt, include a short summary in your pull request describing:

- What changed.
- Why it changed (what problem it solves).
- How to validate it (what a good output should include).

If the change is substantial, add or update an example.

## How to propose changes

### Option A: Open an issue

Open an issue when you are not sure about the solution yet. Include:

- What you are trying to improve.
- The target user and scenario.
- The model and tool used (if relevant).
- Example inputs and what went wrong.
- The expected outcome and success criteria.

### Option B: Open a pull request

Use a pull request when you have a concrete change.

## Pull request process

1. Fork the repository.
2. Create a branch with a descriptive name, for example `add-chatgpt-prd-prompt`.
3. Make changes and keep commits focused.
4. Run a quick self-review using the checklist below.
5. Open a pull request and describe the change clearly.

### Pull request checklist

- [ ] File names follow repo conventions.
- [ ] Prompt follows the standard prompt format.
- [ ] Links are valid.
- [ ] No sensitive data included.
- [ ] Example added or updated when helpful.
- [ ] Content is readable in GitHub Markdown rendering.

## Review criteria

Maintainers will typically review for:

- Practical usefulness for product managers.
- Clarity and completeness of the prompt.
- Reusability across products and industries.
- Output structure that is testable and repeatable.
- Safety and privacy guardrails.

## License

This repository is licensed under the MIT License. By contributing, you agree that your contributions are provided under the same license.

## Attribution and sources

If you borrow ideas from public sources, add a short attribution note in the file under a section named “References". Do not copy large blocks of text. Prefer paraphrasing and original synthesis.

## Security and responsible use

Prompts can influence real decisions. When writing prompts that may touch health, legal, finance, or safety-critical areas:

- Ask for verification steps and a professional review.
- Encourage users to consult qualified professionals.
- Avoid giving definitive diagnoses, legal advice, or instructions that could cause harm.

## Questions

If something in this guide is unclear, open an issue describing what you tried and what you expected.
