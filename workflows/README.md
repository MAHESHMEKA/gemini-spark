# Gemini Spark Workflows

Welcome to the **Workflows** directory! 🔄

A **workflow** represents a complete, multi-step orchestration combining:
- **Tasks** (*What* to accomplish)
- **Schedules** (*When* to run or triggers to listen for)
- **Skills** (*How* each step should be performed)
- **Connected Apps** (Gmail, Google Docs, Google Drive, Google Calendar, etc.)

---

## Example Architecture

```text
[Gmail / Calendar / Drive]
            ↓
          Task
            ↓
        Schedule
            ↓
       Skill + Skill
            ↓
    Structured Output
```

---

## Available Workflows

| Workflow | Description | Connected Apps | Skills Used |
| :--- | :--- | :--- | :--- |
| *(Coming Soon)* | Community contributions welcome! | — | — |

*Browse open issues or submit your own end-to-end workflow!*

---

## How to Contribute a Workflow

1. **Use the Template**: Copy the [Workflow Template](../templates/workflow-template.md).
2. **Document the Pipeline**: Clearly explain the data sources, prerequisite setup, and component skills.
3. **Test End-to-End**: Run the workflow in Gemini Spark to confirm all steps work smoothly together.
4. **File Naming**: Place your workflow in this directory using `kebab-case.md` (e.g., `workflows/morning-executive-briefing.md`).
5. **Open a Pull Request**: Submit your workflow following the guidelines in [CONTRIBUTING.md](../CONTRIBUTING.md).
