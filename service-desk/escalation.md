# IT 140 Service Desk Escalation

Use this page when first-line technical troubleshooting does not resolve the problem or the issue belongs to another support path.

The shared [Escalation Model](../shared/escalation-model.md) defines the common evidence package. This page applies that model to the IT Service Desk role.

## Before Escalating

Confirm that you have:

- classified the problem;
- protected the student's work;
- checked whether the student can continue in the CVD;
- followed the current course/script remediation where appropriate;
- collected the relevant summary/log/support artifact; and
- removed or protected private/security-sensitive information.

## Service Desk Evidence Package

Use the following structure in the ticket or handoff:

```text
IT 140 escalation

User role:
Module/activity:
Issue category:

Environment:
Operating system/version:
Supported or manual configuration:

Repository name (if applicable):
GitHub owner (if applicable):
Local path (if applicable):

Guide/step:
Action attempted:
Expected result:
Actual result:

Lifecycle stage (if applicable):
Final summary/result:
Exit code:
Log/support artifact path:

Troubleshooting already attempted:
CVD continuity available: Yes / No / Not applicable

Attachments:
- Relevant log or sanitized support artifact
- Screenshot, if useful

Private/security information removed or sent through an authorized channel: Yes
```

Omit fields that do not apply; do not guess missing values.

<!-- screenshot placeholder; show a model Service Desk ticket with the IT 140 environment, failed step, exact summary, exit code, and attached sanitized support artifact fields visible -->

## Route to Faculty

Route to faculty when the technical environment works and the primary question is about:

- assignment requirements;
- what must be submitted;
- grading or rubric application;
- instructor feedback;
- course deadlines or instructor-controlled processes; or
- other instructional matters that require faculty authority.

Do not interpret or override the D2L Brightspace Guidelines and Rubric from a Service Desk ticket.

## Route to LSS

Route or refer to Learning Support Specialists (LSS) when the environment works and the student needs learning support with:

- programming concepts;
- understanding syntax/errors in student-created code;
- debugging strategy;
- pseudocode/flowchart reasoning; or
- development of the student's own solution.

Do not provide a complete graded solution through the technical support process.

## Course Technical Maintenance Escalation

Escalate to the course technical maintenance path when evidence indicates a defect in course-managed technical content rather than an individual user's normal environment.

Examples:

- current public README command fails as written;
- a course lifecycle script fails reproducibly in the supported environment;
- a controlled manifest/schema or course asset is invalid;
- a public starter file/test is missing or malformed;
- course automation and documentation disagree;
- the same supported-environment failure affects multiple users; or
- the reference CVD reproduces the course-tool failure.

Before escalation:

1. Check [Course Status](https://github.com/GC-STEM/it140/wiki/Course-Status).
2. Capture exact reproduction steps.
3. Include script version/Version DTG when shown.
4. Include the final summary and exit code.
5. Attach the relevant sanitized support artifact or reviewed log when appropriate.
6. State whether the problem reproduces in the CVD.

A public GitHub Issue can be appropriate for a reproducible defect in public course content **only when the report contains no protected/private information or graded student solution**.

- [Main IT 140 Issues](https://github.com/GC-STEM/it140/issues) — course-wide automation or repository issue
- [Module One Setup Tasks Issues](https://github.com/GC-STEM/it140-m1-setup-tasks/issues) — setup instructions or platform-specific setup behavior

<!-- internal routing placeholder; add approved SNHU internal queue/category/contact for IT 140 course technical maintenance when established -->

## University-System or Account Escalation

For SNHU account, Brightspace, Codio access, device-management, or other university-system problems, use the approved internal Service Desk escalation path for that system.

Do not move an account-specific case into a public GitHub Issue merely because IT 140 uses GitHub or Codio.

<!-- internal routing placeholder; add approved ServiceNow categories/assignment groups for Brightspace, Codio, account, and managed-device cases -->

## GitHub Account/Service Escalation

Separate these two cases:

### Account/Authentication Problem

Examples:

- user cannot access the intended GitHub account;
- GitHub requires account recovery;
- authentication is blocked outside the IT 140 scripts.

Use the appropriate account/service support path. Do not request credentials or recovery secrets.

### Course Workflow/Repository Problem

Examples:

- the current activity template command fails;
- a GC-STEM repository is missing or malformed;
- course documentation creates an incorrect remote/repository state.

Use the course technical maintenance path when the problem is reproducible and course-provided.

## Public Versus Internal Evidence

A public GitHub report may contain:

- public repository URL;
- reproducible public command;
- sanitized error/summary;
- course script version;
- non-sensitive platform information.

Keep these in authorized internal channels instead:

- student-identifying information;
- private repository content;
- student source code unless specifically required and appropriately protected;
- account identifiers not needed publicly;
- credentials or authentication data;
- confidential SNHU infrastructure/routing details.

## Escalation Completion Criteria

A handoff is ready when the receiving role can determine:

- the failing layer;
- the environment and exact procedure;
- what has already been tried;
- the authoritative evidence;
- whether the student has a course-continuity path; and
- what action is requested from the receiving role.
