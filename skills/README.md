# Gemini Spark Skills

Welcome to the **Skills** directory! 🧩

In Gemini Spark, a **skill** defines **how** Gemini should perform a specific type of work. While a **task** defines *what* to do and a **schedule** defines *when* to do it, a skill teaches Gemini reusable methodologies, heuristics, formatting rules, and behaviors.

---

## How Skills Work

Skills can be referenced in tasks or interactive conversations using the slash-command syntax:
```text
/skill-name
```

Combining tasks and skills allows you to build modular, maintainable automations without repeating extensive instructions across every task.

---

## Available Skills

| Skill | Description | Slash Command | Category |
| :--- | :--- | :--- | :--- |
| *(Coming Soon)* | Community contributions welcome! | — | — |

*Browse open issues or submit your own reusable skill!*

---

## How to Contribute a Skill

We welcome new skills across email management, writing, developer workflows, productivity, research, and analysis.

1. **Use the Template**: Copy the [Skill Template](../templates/skill-template.md).
2. **Focus on Reusability**: Ensure the skill teaches a general, reusable capability rather than a one-off single task.
3. **Test in Spark**: Verify the skill in the Gemini Spark interface to ensure it behaves consistently.
4. **File Naming**: Place your skill in this directory using `kebab-case.md` (e.g., `skills/code-review.md`).
5. **Open a Pull Request**: Submit your skill following the guidelines in [CONTRIBUTING.md](../CONTRIBUTING.md).
