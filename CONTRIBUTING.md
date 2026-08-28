# Contributing to Gemini Spark

Thank you for your interest in contributing to **Gemini Spark**! 🎉

This repository is an open-source, community-driven collection of ready-to-use **Gemini Spark tasks, skills, workflows, and guides**. We welcome contributions from everyone—whether you are sharing your first task prompt, writing a reusable skill, fixing a typo, or sharing a complete automation workflow.

---

## Code of Conduct

By participating in this project, you agree to abide by our [Code of Conduct](CODE_OF_CONDUCT.md). Please read it to understand our community standards.

---

## Ways to Contribute

You can contribute in many ways:

1. **Submit a New Task Prompt**: Add a structured prompt for a recurring schedule or event monitor.
2. **Submit a Reusable Skill**: Add a skill prompt teaching Gemini *how* to perform a specific capability.
3. **Submit a Workflow**: Share an end-to-end guide orchestrating multiple tasks, schedules, and skills.
4. **Improve Existing Prompts**: Refine wording, enhance clarity, reduce hallucination risk, or improve output formatting.
5. **Improve Documentation**: Fix errors, clarify setup steps, or add practical tips.
6. **Report Issues or Ideas**: Open an issue if you encounter problems with a prompt or have an idea for a new workflow.

---

## Getting Started

### 1. Contribution Workflow

```text
1. Fork this repository to your GitHub account
       ↓
2. Clone your fork locally
       ↓
3. Create a descriptive branch (e.g., feat/add-calendar-task)
       ↓
4. Author your task, skill, or documentation using our templates
       ↓
5. Test the prompt in the Gemini Spark interface
       ↓
6. Commit your changes with a clear message
       ↓
7. Push your branch and open a Pull Request
```

### 2. File Organization & Naming

* **Tasks**: Place task prompts in the `tasks/` directory using `kebab-case.md` (e.g., `tasks/calendar-prep.md`).
* **Skills**: Place reusable skill definitions in the `skills/` directory using `kebab-case.md` (e.g., `skills/email-analysis.md`).
* **Workflows**: Place multi-step workflow guides in the `workflows/` directory using `kebab-case.md` (e.g., `workflows/morning-briefing.md`).
* **Templates**: Reference the starter templates in [`templates/`](templates/).

---

## Guidelines for Submissions

### A. General Quality Standards

* **Tested**: Always test your task prompt or skill directly in Gemini Spark before submitting. Mention any caveats or quirks observed during testing.
* **Practical & Reusable**: Design prompts that solve real problems and can be easily adapted by others.
* **Clear & Well-Structured**: Include instructions, recommended schedules, customization guidelines, and expected output examples.
* **No Unnecessary Infrastructure**: Keep submissions as clean, standard Markdown. Do not introduce external scripts, custom dependencies, or complex tooling.

### B. Safety, Privacy & Security (Critical)

> [!CAUTION]
> **Never commit personal data, credentials, or private information.**

Ensure all prompts and examples are completely sanitized:
* ❌ No real email addresses, phone numbers, or physical addresses.
* ❌ No passwords, API keys, or authentication tokens.
* ❌ No real private email conversations or sensitive personal documents.
* ✅ Use bracketed placeholders: `[YOUR_EMAIL]`, `[RECIPIENT_NAME]`, `[COMPANY_NAME]`.

### C. Using the Contribution Templates

Please use the provided markdown templates when creating new resources:

* **Task Template**: [`templates/task-template.md`](templates/task-template.md)
* **Skill Template**: [`templates/skill-template.md`](templates/skill-template.md)
* **Workflow Template**: [`templates/workflow-template.md`](templates/workflow-template.md)

---

## Pull Request Checklist

Before submitting your pull request, please verify:

- [ ] I have tested this prompt/skill/workflow in Gemini Spark.
- [ ] I have sanitized all personal information and used clear placeholders (e.g., `[YOUR_NAME]`).
- [ ] I followed the appropriate template format in [`templates/`](templates/).
- [ ] My file is placed in the correct directory (`tasks/`, `skills/`, `workflows/`, or `setup/`).
- [ ] I have used `kebab-case` for newly created filenames.
- [ ] I have linked any related issues in the PR description.

---

## Questions or Need Help?

Feel free to open an issue or start a discussion. We're happy to help you get your contribution ready!
