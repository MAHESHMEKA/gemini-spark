# Setting Up Gemini Spark

> A practical guide to getting **Gemini Spark** ready for tasks, schedules, skills, and automated workflows.

Gemini Spark is designed to manage ongoing tasks and workflows in Gemini. You can define **what** you want Gemini to do with a task, **when** it should run with a schedule, and **how** it should perform a type of work with a skill.

This guide walks through the initial setup and then shows how to create your first useful Spark workflow.

---

## Table of Contents

* [1. Prerequisites](#1-prerequisites)
* [2. Open Gemini Spark](#2-open-gemini-spark)
* [3. Understand the Spark Building Blocks](#3-understand-the-spark-building-blocks)
* [4. Connect Gmail and Google Workspace](#4-connect-gmail-and-google-workspace)
* [5. Create Your First Task](#5-create-your-first-task)
* [6. Add a Schedule](#6-add-a-schedule)
* [7. Create and Use Skills](#7-create-and-use-skills)
* [8. Try the Gmail Report Task](#8-try-the-gmail-report-task)
* [9. Test a Scheduled Task](#9-test-a-scheduled-task)
* [10. Manage Tasks and Schedules](#10-manage-tasks-and-schedules)
* [11. Troubleshooting](#11-troubleshooting)
* [12. Recommended Workflow](#12-recommended-workflow)
* [13. Security and Privacy](#13-security-and-privacy)
* [14. Next Steps](#14-next-steps)

---

# 1. Prerequisites

Before setting up Gemini Spark, make sure you have:

* A **personal Google Account**
* A supported Google AI subscription
* **Keep Activity** turned on
* Access to Gemini Spark in your region
* A supported Gemini app or the Gemini web app

Google currently states that Spark requires users to be **18 or older**, signed in with a personal Google Account, and have a supported Google AI Pro or Ultra subscription. Spark is currently available in supported regions and is accessible through the Gemini web app, Gemini mobile app, and Gemini app on Mac.

> **Note:** Availability, subscription requirements, regional availability, and interface details can change. Check Google's current Gemini Help documentation if something in the interface differs from this guide.

---

# 2. Open Gemini Spark

## On the Web

1. Open the Gemini web app.
2. Sign in with your Google Account.
3. Open the sidebar.
4. Select **Switch to Spark**.
5. Select **Use Gemini Spark** if prompted.

Google's current Spark interface provides dedicated areas for **Tasks**, **Schedules**, and **Skills**.

---

# 3. Understand the Spark Building Blocks

Before creating automations, it helps to understand the three core concepts.

| Component    | Purpose                                        | Simple Example                     |
| ------------ | ---------------------------------------------- | ---------------------------------- |
| **Task**     | Defines **what** Gemini should accomplish      | "Create a daily Gmail report"      |
| **Schedule** | Defines **when** the task runs                 | "Every day at 6:00 AM"             |
| **Skill**    | Defines **how** Gemini performs a type of work | "Analyze emails using these rules" |

Think of a Spark workflow like this:

```text
                    GEMINI SPARK
                         │
            ┌────────────┼────────────┐
            │            │            │
          TASK        SCHEDULE       SKILL
           │             │            │
         WHAT           WHEN          HOW
           │             │            │
           └─────────────┼────────────┘
                         │
                    WORKFLOW
                         │
                         ▼
                  Gemini executes it
```

Google describes these three building blocks as the **what, when, and how** of Spark workflows.

---

# 4. Connect Gmail and Google Workspace

Some Spark workflows need access to Google Workspace data such as:

* Gmail
* Google Drive
* Google Docs
* Google Calendar
* Google Tasks
* Google Keep

For example, the Gmail report task in this repository needs access to Gmail.

## Connect Google Workspace

1. Open Gemini.
2. Make sure you're signed in with the **same Google Account that contains your Gmail**.
3. Ask Gemini to access information from Google Workspace.
4. If Google Workspace is not connected, Gemini should provide an option to connect it.
5. Follow the on-screen instructions.
6. Grant the required permissions.

Google's Workspace connection allows Gemini to retrieve information from services such as Gmail, Docs, and Drive. Google also notes that **Keep Activity must be enabled** for the Workspace connection.

### Important

Use the same Google Account for:

```text
Google Account
      │
      ├── Gmail
      ├── Google Workspace
      └── Gemini Spark
```

Using a different account can prevent Spark from accessing the Gmail or Workspace information you expect.

---

# 5. Create Your First Task

There are two useful ways to create a Spark task.

## Method 1 — Create Conversationally

This is usually the easiest method.

1. Open Gemini Spark.
2. Start a new task.
3. Describe exactly what you want Gemini to accomplish.
4. Include important requirements, constraints, and output formatting.
5. Submit the task.

For example:

```text
Create a daily task that reviews my Gmail,
identifies important emails, summarizes them,
and tells me which emails require action.
```

Spark can then help you develop the task.

Google also recommends using phrases such as:

```text
set up
get started
interview me
```

when asking Spark to help configure a new task or skill.

---

## Method 2 — Build From a Repository Prompt

This repository is designed to make this workflow easier.

For example:

```text
Repository
   │
   ▼
tasks/gmail_report.md
   │
   ▼
Copy the prompt
   │
   ▼
Paste into Gemini Spark
   │
   ▼
Customize
   │
   ▼
Create Task
   │
   ▼
Add Schedule
```

This makes the repository useful as a library of **copy-paste-ready Spark workflows**.

---

# 6. Add a Schedule

A schedule tells Spark **when to execute a task**.

Gemini currently supports time-based schedules such as:

* Once
* Hourly
* Daily
* Weekly
* Monthly
* Yearly

Spark also supports event-based monitoring such as Gmail and topic monitors.

## Create a Schedule Conversationally

While creating your Spark task, you can simply specify the timing in your instructions.

Example:

```text
Every day at 6:00 AM,
review my Gmail and create a daily report.
```

Spark can interpret the scheduling requirement and create the associated schedule.

---

## Create a Schedule Manually

For a time-based schedule:

1. Open Gemini Spark.
2. Open **Schedules**.
3. Select **Create manually**.
4. Enter a schedule name.
5. Select when the task should run.
6. Enter the task instructions.
7. Create the schedule.

Google's current interface saves created schedules under the **Ongoing** section.

---

## Time Zones

Time-based schedules are associated with the time zone in which they were created.

For example:

```text
Created in India
       │
       ▼
IST (UTC+5:30)
       │
       ▼
6:00 AM schedule
```

If you later travel to another time zone, the schedule does not automatically become 6:00 AM in the new local time. Google advises editing the schedule if you want it adjusted to a new time zone.

---

# 7. Create and Use Skills

A **skill** is a reusable set of instructions and context that teaches Gemini how to perform a particular type of work. Skills can be used independently or combined with other skills.

A useful mental model is:

```text
Task
"What should I accomplish?"

        +

Schedule
"When should it happen?"

        +

Skill
"How should it be done?"
```

## Create a Skill

You can ask Spark to create one conversationally.

Example:

```text
Create a skill for analyzing incoming emails.

The skill should:
- identify important messages
- detect deadlines
- identify required actions
- classify priority
- avoid unnecessary noise
- produce concise summaries
```

Spark can create the skill and save it to the Skills area.

---

## Use an Existing Skill

When creating a task, you can reference an existing skill using `/` and then select the skill.

For example:

```text
/gmail-analysis
```

You can also combine multiple skills in one task when a workflow requires several capabilities.

---

# 8. Try the Gmail Report Task

This repository currently contains its first example task:

## Gmail Daily Report

[`tasks/gmail_report.md`](../tasks/gmail_report.md)

The task is designed to create a daily Gmail report containing:

```text
                    Gmail
                      │
                      ▼
              Email Analysis
                      │
            ┌─────────┼─────────┐
            ▼         ▼         ▼
         HIGH      MEDIUM    REPLY
        PRIORITY   PRIORITY   REQUIRED
            │         │         │
            └─────────┼─────────┘
                      ▼
              Quick Action List
```

It focuses especially on:

* Important unread messages
* Google Careers and job opportunities
* Interview and application updates
* Payments and financial notifications
* Deadlines
* Security/account alerts
* Emails requiring action
* Emails requiring a reply

It also generates suggested replies when a response is genuinely required.

### Recommended Schedule

The example is designed around:

```text
Every day
    ↓
6:00 AM
    ↓
India Standard Time (IST)
```

You can change the schedule to suit your own routine.

---

## How to Set It Up

1. Open [`tasks/gmail_report.md`](../tasks/gmail_report.md).
2. Copy the complete prompt.
3. Open Gemini Spark.
4. Create a new task.
5. Paste the prompt.
6. Customize anything that is specific to your workflow.
7. Create or confirm the schedule.
8. Make sure Gmail/Google Workspace access is available.
9. Test the task before relying on it.

---

# 9. Test a Scheduled Task

Before depending on an automated workflow, test it.

For time-based schedules, Google currently provides a **Run now** option from the Schedules interface.

A good testing process is:

```text
Create Task
    │
    ▼
Create Schedule
    │
    ▼
Run Now
    │
    ▼
Review Output
    │
    ▼
Fix Prompt
    │
    ▼
Test Again
    │
    ▼
Enable Regular Schedule
```

Pay particular attention to:

* Whether the correct data is being accessed
* Whether important items are classified correctly
* Whether irrelevant information is excluded
* Whether deadlines are detected
* Whether actions are clearly identified
* Whether output formatting is easy to scan
* Whether any assumptions are being invented

---

# 10. Manage Tasks and Schedules

## Tasks

You can view your Spark task threads from the **Tasks** section.

From there you can review:

* Recent tasks
* Task progress
* Task conversations
* Task outputs

Google currently provides a Tasks area in the Spark sidebar for managing these threads.

---

## Schedules

Schedules can be reviewed from the **Schedules** area.

Schedules are organized into states such as:

```text
Ongoing
Paused
Completed
```

You can:

* View schedules
* Edit schedules
* Pause schedules
* Resume schedules
* Delete schedules

You can also ask Gemini to edit a schedule from its related task thread.

---

# 11. Troubleshooting

## Spark Does Not Appear

Check:

* You are signed in with the correct Google Account.
* Your account meets the current Spark requirements.
* Gemini Spark is available in your region.
* You have an eligible subscription.
* Keep Activity is enabled.

Spark availability and requirements are controlled by Google and may change.

---

## Gmail Cannot Be Accessed

Check:

1. Gemini is signed in to the correct Google Account.
2. Google Workspace is connected.
3. Keep Activity is enabled.
4. Gmail/Workspace permissions were granted.
5. Your Gmail account is actually the account connected to Gemini.

Google notes that work or school accounts can also require administrator support before Workspace connections can be enabled.

---

## Schedule Does Not Run

Possible causes include:

* Usage limits
* Too many concurrently running tasks
* Temporary service delays
* The schedule being paused
* The task being completed
* Incorrect or missing schedule configuration

Google currently documents a limit of **50 active schedules** and up to **15 tasks running concurrently**. Scheduled runs can also be delayed during periods of high traffic.

---

## Schedule Runs at a Slightly Different Time

Scheduled task execution is not necessarily exact to the second.

Google notes that scheduled task run times are approximate and may be delayed under some conditions.

For workflows that require truly time-critical execution, do not assume a Spark schedule behaves like a precise cron job.

---

# 12. Recommended Workflow

For larger workflows, use a layered design instead of putting everything into one enormous prompt.

### Recommended architecture

```text
                    ┌───────────────┐
                    │    SCHEDULE   │
                    │     WHEN?     │
                    └───────┬───────┘
                            │
                            ▼
                    ┌───────────────┐
                    │      TASK     │
                    │     WHAT?     │
                    └───────┬───────┘
                            │
                    ┌───────┴───────┐
                    ▼               ▼
             ┌────────────┐  ┌────────────┐
             │   SKILL    │  │   SKILL    │
             │    HOW?    │  │    HOW?    │
             └─────┬──────┘  └─────┬──────┘
                   │               │
                   └───────┬───────┘
                           ▼
                       WORKFLOW
```

For example:

```text
Schedule
"Every morning at 6:00 AM"

        ↓

Task
"Generate my daily Gmail report"

        ↓

Skill
"Analyze and classify email"

        ↓

Skill
"Draft professional replies"

        ↓

Output
"Daily Gmail Summary"
```

This approach makes workflows easier to understand, maintain, reuse, and improve.

---

# 13. Security and Privacy

Treat Spark tasks and skills like software configuration.

Never put secrets into repository files.

Do **not** commit:

```text
❌ Passwords
❌ API keys
❌ Authentication tokens
❌ Private email contents
❌ Personal credentials
❌ Recovery codes
❌ Sensitive account information
```

When sharing a workflow publicly, replace personal information with placeholders.

For example:

```text
❌ Send the report to mahesh@example.com

✅ Send the report to [YOUR_EMAIL]
```

Also avoid copying real private email contents into task examples.

---

# 14. Next Steps

Once Gemini Spark is working, explore the rest of this repository.

### Tasks

Browse:

[`tasks/`](../tasks/)

Find ready-to-use task prompts and workflows.

### Skills

Browse:

[`skills/`](../skills/)

Explore reusable instructions for specific types of work.

### Workflows

Browse:

[`workflows/`](../workflows/)

Explore complete multi-step Spark workflows.

### Contribute

Have a useful workflow?

See the repository contribution guidelines and help expand the collection.

---

# Quick Start

For users who just want to get started:

```text
1. Open Gemini
       ↓
2. Switch to Spark
       ↓
3. Connect Google Workspace if needed
       ↓
4. Choose/create a Task
       ↓
5. Add a Schedule
       ↓
6. Add relevant Skills
       ↓
7. Run a test
       ↓
8. Review the output
       ↓
9. Enable the recurring workflow
```

---

## First Recommended Task

Start with:

**[`tasks/gmail_report.md`](../tasks/gmail_report.md)**

It provides a practical example of combining:

```text
Task
+
Schedule
+
Gmail
+
Structured analysis
+
Action detection
+
Reply drafting
```

This is a good starting point for understanding how Gemini Spark can turn a simple prompt into a recurring workflow.
