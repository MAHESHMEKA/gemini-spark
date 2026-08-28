# Daily Gmail Summary — Gemini Spark Scheduled Task

A scheduled Gemini Spark task that reviews Gmail every morning and produces a concise, action-oriented email summary.

## Schedule

* **Frequency:** Daily
* **Time:** 6:00 AM
* **Timezone:** India Standard Time (IST, UTC+5:30)

## Task Prompt

> Every day at **6:00 AM India Standard Time (IST, UTC+5:30)**, search my Gmail and generate a **Daily Gmail Summary Report**.

### 1. Email Scanning

* Review **all relevant recent emails**, with **unread emails as the highest priority**.
* Do not limit the analysis only to unread emails if an important older email requires attention.
* Identify emails that:

  * Require action
  * Contain deadlines
  * Involve payments or financial activity
  * Relate to jobs or career opportunities
  * Contain account or security alerts
  * Require a response
  * Are otherwise important or time-sensitive
* Avoid cluttering the report with obvious:

  * Promotional emails
  * Newsletters
  * Social notifications
  * Routine automated notifications
  * Low-value marketing messages
* Exclude low-value emails unless they contain information that requires action.
* Group duplicate or repeated notifications when appropriate instead of listing the same information multiple times.

---

## 2. Priority Classification

### 🔴 High Priority

Include emails that are **urgent, important, time-sensitive, financially significant, career-related, security-related, or likely to require action**.

Examples include:

* **Google Careers / job opportunities**
* Job application updates
* Interview invitations
* Interview schedules
* Coding tests or assessments
* Recruiter messages
* Offer letters
* Hiring or application deadlines
* **Payment-related emails**
* Payments due
* Failed payments
* Refunds
* Transactions
* Invoices
* Bills
* Subscription renewals
* Financial alerts
* **Deadline-related emails**
* Application deadlines
* Assignment deadlines
* Registration deadlines
* Payment deadlines
* Interview deadlines
* Expiring offers
* Account or security alerts
* Password changes
* Suspicious activity
* Verification requests
* Important access-related notifications
* Important academic, professional, government, or administrative communications
* Any email where ignoring it could cause:

  * A missed opportunity
  * Financial loss
  * A penalty
  * A missed deadline
  * Account problems
  * Other meaningful consequences

For every **High Priority** email, use this format:

```text
Subject: [Gmail subject]

Summary:
[Explain the email in 2–3 concise lines, focusing on the important information.]

Action needed: [Yes / No]

Deadline: [Mention the deadline/date when available]
```

---

### 🟡 Medium Priority

Include emails that are **useful or potentially important but are not urgent** and do not require immediate attention.

For every **Medium Priority** email, use this format:

```text
Subject: [Gmail subject]

Summary:
[Explain the email in 2–3 concise lines.]

Action needed: [Yes / No]
```

---

## 3. ✉️ Reply Required

Create this section **only when a reply is genuinely needed**.

Do **not** include:

* Automated notifications
* Newsletters
* Promotional emails
* Receipts
* FYI-only messages
* Emails where no response is expected

For each email that genuinely requires a response, use this format:

```text
Subject: [Gmail subject]

Why a reply is needed:
[Briefly explain why I should respond.]

Suggested reply:

[Draft a natural, clear, professional reply here.]
```

### Reply Draft Rules

The suggested reply must:

* Directly address the sender's message.
* Be concise but complete.
* Match the tone of the original email.
* Avoid inventing facts, commitments, dates, or information that are not known.
* Clearly indicate anything I need to fill in manually.
* Be suitable as a starting draft that I can review, modify, and send myself.

---

## 4. Report Format

Start every report with:

```markdown
# Daily Gmail Summary — [Date]
```

Then organize the report as follows:

```markdown
## 🔴 High Priority

[Important emails]

## 🟡 Medium Priority

[Useful but non-urgent emails]

## ✉️ Reply Required

[Only include this section when a reply is genuinely required.]

## ✅ Quick Action List

[Short checklist of the most important actions I should take today, ordered by urgency.]
```

---

## 5. Quick Action List

At the end of the report, provide a concise checklist containing the **most important actions I should take today**.

Order the actions by urgency and importance.

Example:

```text
## ✅ Quick Action List

- [ ] Submit Google application before 11:59 PM
- [ ] Complete interview assessment
- [ ] Pay pending subscription invoice
- [ ] Reply to recruiter regarding interview availability
```

Do not include unnecessary actions merely to make the checklist longer.

---

## 6. Important Rules

### Prioritize Actionability

Prioritize emails based on **importance and required action**, not simply the number of emails received.

### Read Email Content

When possible, analyze the **actual email content**, not just the subject line.

### Pay Special Attention To

Be especially careful with:

* Deadlines
* Payments
* Jobs
* Interviews
* Applications
* Security alerts
* Account issues
* Time-sensitive requests

### Clearly Identify Actions

Always distinguish between:

* `Action needed: Yes`
* `Action needed: No`

When action is required, explain **what action is needed**.

### Reply Section

* Show **Reply Required** only when a genuine response is expected.
* If no emails require a reply, **omit the section entirely**.

### Empty Categories

If there are no high-priority or medium-priority emails, explicitly state that there are none.

Do not fill categories with irrelevant emails just to populate the report.

### Keep It Concise

The report should be:

* Easy to scan
* Concise
* Action-oriented
* Useful for a quick morning review

Focus on **what matters and what I need to do**, rather than providing lengthy explanations.

### Do Not Modify Gmail

**Never perform any Gmail actions.**

Only analyze and report.

Do **not**:

* Send emails
* Reply to emails
* Forward emails
* Delete emails
* Archive emails
* Mark emails as read
* Mark emails as unread
* Move emails
* Modify labels
* Change email settings

The task should **only read/analyze emails and prepare the report and reply drafts**.
