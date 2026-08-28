# Gemini Spark

> An open-source, community-driven collection of **Gemini Spark tasks, skills, prompts, workflows, and setup guides** for developers and Gemini Spark users.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Contributions Welcome](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](CONTRIBUTING.md)

[Visit Tasks (gmail_report task)](tasks/gmail_report.md)

## About

**Gemini Spark** is a personal AI agent from Google that can manage tasks, run scheduled workflows, and use reusable skills.

This repository is a community-driven collection of **ready-to-use resources for Gemini Spark users**.

The goal is simple:

> **Make Gemini Spark easier to set up, easier to use, and more powerful through reusable community-created tasks, skills, and workflows.**

Whether you're experimenting with your first Spark task or building advanced automated workflows, this repository aims to give you practical starting points that you can copy, customize, and improve.

---

## What You'll Find Here

### ⚡ Task Prompts

Ready-to-use prompts for creating useful Gemini Spark tasks.

Examples include:

* Gmail reports
* Productivity workflows
* Research tasks
* Daily/weekly summaries
* Career and job tracking
* Personal organization
* Information monitoring
* Developer workflows
* Custom automation ideas

Currently available:

| Task                                    | Description                                                                             |
| --------------------------------------- | --------------------------------------------------------------------------------------- |
| [`gmail-report`](tasks/gmail_report.md) | Daily Gmail analysis with priority classification, action detection, and reply drafting |

More tasks will be added as the repository grows.

---

### 🧩 Skills

Reusable Gemini Spark skills designed to teach Spark **how** to perform a specific type of work.

Skills can be combined with tasks to create more sophisticated workflows.

Planned skill categories include:

* Email
* Research
* Writing
* Coding
* Productivity
* Data analysis
* Career workflows
* Personal organization
* Developer workflows

---

### 🛠️ Setup Guides

Documentation for getting started with Gemini Spark, including:

* Spark setup
* Creating your first task
* Creating schedules
* Creating and using skills
* Connecting supported services
* Building reusable workflows
* Tips and best practices
* Troubleshooting common problems

---

### 🔄 Workflows

Complete examples showing how multiple Gemini Spark capabilities can work together.

For example:

```text
Gmail
  ↓
Task
  ↓
Skill
  ↓
Analyze emails
  ↓
Identify important items
  ↓
Generate summary
  ↓
Prepare reply drafts
```

The repository will gradually include more complete, real-world workflows contributed by the community.

---

## Repository Structure

The repository is intentionally kept simple while the project is growing.

```text
gemini-spark/
│
├── README.md
├── LICENSE
│
├── tasks/
│   └── gmail-report.md
│
├── skills/
│   └── ...
│
├── setup/
│   └── ...
│
└── workflows/
    └── ...
```

### Directory Guide

| Directory    | Purpose                                |
| ------------ | -------------------------------------- |
| `tasks/`     | Ready-to-use Gemini Spark task prompts |
| `skills/`    | Reusable Spark skills                  |
| `setup/`     | Setup and configuration guides         |
| `workflows/` | Complete workflow examples             |

As the project grows, additional categories may be introduced when they provide clear value.

---

# Getting Started

## 1. Explore the Repository

Start by browsing the available tasks and skills.

```text
tasks/
skills/
setup/
workflows/
```

Choose something relevant to your workflow and adapt it to your needs.

---

## 2. Use a Task

Open a task file such as:

```text
tasks/gmail-report.md
```

Copy the prompt and use it when creating your Gemini Spark task.

Customize details such as:

* Schedule
* Output format
* Priority rules
* Personal preferences
* Connected apps
* Required actions

---

## 3. Create a Skill

Skills are useful when you want to define a reusable way of performing a particular type of work.

Instead of repeating the same instructions across multiple tasks, create a skill once and reuse it wherever appropriate.

---

## 4. Build Your Own Workflow

A powerful Spark workflow can combine:

```text
Task
  +
Schedule
  +
Skill
  +
Connected Apps
```

Start simple and gradually make the workflow more sophisticated.

---

# Tasks vs Skills vs Schedules

Gemini Spark uses these concepts for different purposes:

| Concept      | Purpose                                              |
| ------------ | ---------------------------------------------------- |
| **Task**     | Defines **what** Gemini should accomplish            |
| **Schedule** | Defines **when** the task should run                 |
| **Skill**    | Defines **how** Gemini should perform a type of work |

For example:

```text
TASK
"Create a daily Gmail report"

        ↓

SCHEDULE
"Run every day at 6:00 AM"

        ↓

SKILL
"Analyze emails and identify priority/action items"
```

This repository focuses primarily on building and sharing these reusable building blocks.

---

# Contributing

Contributions are welcome! ❤️

This project is intended to be built **with the Gemini Spark community**, not just for it.

You can contribute in any way that helps improve the repository.

### Ways to Contribute

You can:

* Submit new task prompts
* Submit new skills
* Improve existing prompts
* Improve documentation
* Fix mistakes
* Report bugs or unexpected behavior
* Suggest new features
* Suggest new task or skill categories
* Share your Gemini Spark workflows
* Improve examples
* Improve repository organization
* Test existing resources
* Share practical tips and best practices

Even small improvements are valuable.

---

## How to Contribute

The basic workflow is:

```text
1. Fork this repository
        ↓
2. Create a branch
        ↓
3. Make your changes
        ↓
4. Test your task / skill / documentation
        ↓
5. Commit your changes
        ↓
6. Open a Pull Request
```

A simple contribution is perfectly fine:

> **Fork → Make changes → Open a Pull Request**

---

# Contribution Guidelines

To keep the repository useful and maintainable, please try to make contributions:

### Clear

Explain what the task, skill, or workflow is designed to accomplish.

### Reusable

Prefer prompts that can be adapted by other users rather than highly personal instructions.

### Practical

Resources should solve a real problem or demonstrate a useful Spark capability.

### Tested

Whenever possible, test a task or skill before submitting it.

Mention any important limitations or assumptions.

### Well Documented

A useful task should ideally explain:

* What it does
* Who it is useful for
* How to use it
* What needs to be customized
* Expected output
* Important limitations

### Safe

Do not include:

* Passwords
* API keys
* Personal credentials
* Private email content
* Personal account information
* Sensitive data
* Other secrets

Never commit private information to the repository.

---

# Task Prompt Guidelines

When submitting a new task, prefer a structure similar to:

```markdown
# Task Name

## Purpose

Explain what the task does.

## Recommended Schedule

Explain when/how often it can be run.

## Prompt

[Complete copy-paste-ready prompt]

## Customization

Explain what users may want to change.

## Expected Output

Show an example of the expected result.

## Notes

Include limitations, assumptions, or important considerations.
```

The goal is to make every task **copy-pasteable while still being understandable and customizable**.

---

# Skill Guidelines

Skills should generally focus on **one reusable capability**.

A good skill should:

* Have a clear purpose
* Provide explicit instructions
* Define expected behavior
* Include useful formatting or workflow rules
* Avoid unnecessary instructions
* Be reusable across multiple tasks

A skill should teach Gemini **how to perform a particular kind of work**, rather than being a one-off task prompt.

---

# Quality Over Quantity

This repository is not intended to become a random collection of prompts.

The goal is to build a library of **high-quality, useful, tested Gemini Spark resources**.

A smaller collection of excellent tasks is more valuable than hundreds of poorly documented prompts.

---

# Roadmap

This roadmap will evolve as the community grows.

### Current

* [x] Repository created
* [x] Initial Gmail report task
* [x] MIT license
* [ ] Initial setup documentation
* [ ] Initial skills collection

### Planned

* [ ] Gemini Spark setup guide
* [ ] Task creation guide
* [ ] Skills guide
* [ ] More ready-to-use task prompts
* [ ] More reusable skills
* [ ] Workflow examples
* [ ] Contribution guide
* [ ] Issue templates
* [ ] Pull request template
* [ ] Troubleshooting guide
* [ ] Community-submitted workflows
* [ ] Better task/skill categorization

The roadmap is community-driven and may change based on what users find most useful.

---

# Ideas for Future Tasks

Some examples of areas that could be useful additions:

```text
📧 Email
   ├── Gmail summaries
   ├── Important email detection
   ├── Follow-up tracking
   └── Reply assistance

💼 Career
   ├── Job opportunity tracking
   ├── Application monitoring
   ├── Interview preparation
   └── Recruiter communication

📚 Learning
   ├── Daily learning plans
   ├── Study summaries
   ├── Research assistants
   └── Revision workflows

💻 Development
   ├── GitHub monitoring
   ├── Coding workflows
   ├── Documentation
   └── Developer productivity

📊 Productivity
   ├── Daily briefings
   ├── Weekly reviews
   ├── Task management
   └── Personal workflows
```

These are examples rather than restrictions. Community members are encouraged to contribute ideas outside these categories.

---

# Project Philosophy

Gemini Spark becomes significantly more useful when people stop thinking only in terms of individual prompts and start thinking in terms of **reusable workflows**.

The vision of this repository is to make those workflows:

**Discoverable → Understandable → Reusable → Customizable → Community-improved**

A useful contribution today can become the foundation for a much better workflow tomorrow.

---

# Community

This repository is built for Gemini Spark users and developers.

Whether you contribute a sophisticated workflow, a tiny improvement to an existing prompt, documentation fixes, testing feedback, or a new idea, your contribution can help make the ecosystem better for everyone.

**Have something useful? Share it.**

---

# Disclaimer

This is an **independent community project**.

It is not affiliated with, sponsored by, or endorsed by Google.

Gemini and Gemini Spark are products/services of Google. Product capabilities, availability, limits, interfaces, and behavior may change over time.

Always review and test a task or skill before relying on it for important workflows.

---

# License

This project is licensed under the **MIT License**.

See [`LICENSE`](LICENSE) for the full license text.

---

## ⭐ Support the Project

If you find this repository useful:

* Star the repository
* Share useful tasks and skills
* Submit improvements
* Open issues for bugs or ideas
* Contribute new workflows
* Help improve the documentation

The best way to support this project is to **use it, improve it, and share what you build with the community**.

---

> **Built by Gemini Spark users, for Gemini Spark users.**
