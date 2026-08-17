# IT 140 Support Boundaries

This page provides a common routing model for IT 140 support.

It helps supporters distinguish among:

- technical environment problems;
- programming and learning-support needs;
- assignment, grading, and instructor questions; and
- academic-advising concerns.

> [!IMPORTANT]
> This page defines the support model used by the IT 140 support repository. Existing SNHU policies, departmental procedures, role definitions, privacy requirements, and escalation channels take precedence where they are more specific.

## Start by Classifying the Problem

A useful first question is:

> **Is the problem about the environment in which the student's work runs, or about the student's work itself?**

Then refine the classification.

### Technical Environment or Access Problem

Examples:

- CVD will not launch;
- VS Code will not start;
- Python cannot run in the supported course IDE;
- GitHub authentication fails;
- GitHub CLI cannot access the student's account;
- the student cannot create or clone the repository as documented;
- Verify reports `NOT COMPLIANT`;
- a course lifecycle script fails;
- a course-provided repository file or tool behaves differently from the documentation.

These problems primarily belong to a **technical support** path.

### Programming or Learning Problem

Examples:

- the Python program runs but gives the wrong result;
- the student does not understand a loop, branch, function, list, or dictionary;
- pseudocode does not match the student's intended logic;
- the student needs help reasoning through an error in their own code;
- the student needs help learning how to test or debug.

These problems primarily belong to a **learning/instructional support** path.

### Assignment or Grading Problem

Examples:

- what must be submitted;
- whether a file meets a rubric criterion;
- a grading decision;
- instructor feedback;
- a deadline;
- an accommodation;
- a submission problem involving course requirements rather than the technical environment.

These questions primarily belong to **faculty/instructor** processes.

### Academic Planning or Referral Problem

Examples:

- whether the course fits a student's academic plan;
- course sequencing;
- broader program questions;
- help identifying the right support resource;
- concerns that require advising rather than technical or instructional troubleshooting.

These primarily belong to **academic advising** processes.

## Primary Support Routing Matrix

| Problem | Primary Support Role | Notes |
| --- | --- | --- |
| CVD access or launch problem | IT Service Desk | Escalate course-specific CVD behavior with evidence when normal access support does not resolve it |
| Supported local course IDE fails to install/configure | IT Service Desk | Use current setup instructions and logs; CVD can provide continuity |
| Verify reports `NOT COMPLIANT` or failures | IT Service Desk | Collect summary and log; escalate course-automation defects when appropriate |
| GitHub account/authentication or `gh` problem | IT Service Desk | Distinguish GitHub account access from a course-repository defect |
| Course template cannot be created/cloned as documented | IT Service Desk | Confirm account, repo owner, repo existence, and current README first |
| Public GC-STEM repository appears broken or inconsistent | Course technical maintainers | A GitHub Issue may be appropriate if the repository directs users there |
| Course-provided script, test, starter file, or documentation appears defective | Course technical maintainers | Preserve reproduction steps and distinguish from student edits |
| Student Python code has syntax or logic problems | Faculty or LSS | Service Desk may isolate environment functionality but should not become the code-solution provider |
| Student needs help understanding programming concepts | Faculty or LSS | Use learning support appropriate to the student's current module |
| Student needs help with pseudocode or flowchart reasoning | Faculty or LSS | Maintain academic-integrity boundaries |
| What the assignment requires or what to submit | Faculty / D2L Brightspace | Guidelines and Rubric are authoritative |
| Grading or instructor feedback | Faculty | Do not reinterpret a grading decision through technical support |
| Academic plan, course sequence, or broader program concern | Academic Advisor | Refer technical or instructional subquestions to the appropriate role |
| Student does not know where to ask for help | Any supporter can triage | Route using this page and the relevant role guide |

## IT Service Desk Boundary

The IT Service Desk should focus on whether the **supported technical environment and access path** are functioning as documented.

Examples of appropriate Service Desk questions:

- Can the student access the system?
- Which environment is being used?
- Does the course IDE launch?
- Does Python run?
- Is GitHub CLI authenticated?
- Is the student working in the correct repository?
- What does Verify report?
- What does the lifecycle summary/log show?
- Can the issue be reproduced in the CVD reference environment?

The Service Desk does **not** need to determine whether a student's algorithm is correct or whether the student's program deserves credit under a rubric.

A program that runs but produces the wrong answer is not automatically an environment failure.

## Faculty Boundary

Faculty are the authoritative course contact for matters such as:

- interpreting the current assignment requirements;
- grading;
- rubric application;
- instructor feedback;
- assignment submission expectations;
- course-content questions appropriate for the instructor; and
- determining what assistance is appropriate for a graded activity.

Faculty may also help triage technical problems, but technical infrastructure diagnosis can be routed to the Service Desk or course technical support when appropriate.

## LSS Boundary

Learning Support Specialists (LSS) help students build understanding and problem-solving skills.

Appropriate LSS support may include:

- explaining course-level programming concepts;
- helping students interpret error messages;
- helping students reason through their own logic;
- teaching debugging and testing approaches;
- helping students use course development tools at a learning-support level; and
- helping students locate relevant course resources.

LSS support should help the student **discover and develop the solution**, not replace the student's graded work with a completed solution.

Technical environment failures that cannot be resolved through ordinary course-tool guidance should be referred through the technical support path.

## Academic Advisor Boundary

Academic advisors need enough technical and course context to:

- set reasonable course expectations;
- recognize when a student's concern is technical, instructional, or academic;
- help a student identify the correct support resource; and
- address academic-planning questions within the advisor role.

Advisors are not expected to troubleshoot Git, Python, VS Code, or course automation.

## Course Technical Maintainer Boundary

Some problems are neither ordinary student-code questions nor routine desktop support.

Examples include:

- a GC-STEM repository contains a broken link or incorrect starter file;
- a current course automation script fails reproducibly in the supported reference environment;
- the manifest/configuration defines an incorrect course component;
- course-provided tests fail against the intended starter state;
- the same supported-environment failure affects multiple users;
- documentation and automation disagree.

These should be escalated to the **course technical maintenance** path with a reproducible evidence package.

See [Escalation Model](escalation-model.md).

## Academic Integrity Boundary

Support is expected to help students make progress without replacing the student's graded work.

Supporters should not:

- post complete solutions to graded IT 140 assignments or projects in public support channels;
- provide a finished graded deliverable when the student's task is to create that deliverable;
- modify a student's program into a completed assignment while presenting the work as the student's own; or
- use a technical-support channel to bypass course academic-integrity expectations.

Supporters may:

- explain concepts;
- ask diagnostic questions;
- point to relevant course resources;
- demonstrate a concept with a different or partial example;
- help a student interpret an error;
- help a student test their own work; and
- help isolate whether a problem is environmental or in student-created code.

Role-specific guides should provide more detailed examples appropriate to that role.

## Technical Versus Student-Code Test

When the distinction is unclear, ask:

1. **Can Python run a simple known-good command or course-provided example in the supported environment?**
2. **Does the course Verify process report an environment failure?**
3. **Does the same student program fail in the CVD reference environment?**
4. **Does only this student's code fail while the environment otherwise works?**

These questions do not prove the cause by themselves, but they help separate environment failures from programming problems.

> [!CAUTION]
> Do not modify or delete the student's work merely to test the environment. Preserve student files and Git history.

## Shared Ownership Cases

Some issues cross role boundaries.

### Example: "My assignment won't run"

Possible routes:

- Python itself cannot run → technical support.
- VS Code is using the wrong interpreter → technical support / course IDE support.
- Python runs but the student's code has a syntax error → faculty or LSS.
- The student does not know which file must be submitted → faculty / Brightspace.
- The starter file itself is malformed for everyone → course technical maintainer.

### Example: "GitHub doesn't work"

Possible routes:

- cannot sign in to GitHub → account/technical support;
- `gh auth status` shows the wrong account → technical/repository workflow support;
- student's private repo already exists → repository workflow issue;
- student is trying to clone the GC-STEM template directly → repository workflow issue;
- GitHub works, but the student does not understand Git concepts → faculty/LSS learning support as appropriate;
- the public course repository is missing or broken → course technical maintainer.

## Public Versus Internal Support Channels

A public GitHub repository may be appropriate for:

- a reproducible defect in a public course repository;
- a broken public documentation link;
- a course-tool issue that does not require private information; or
- a general improvement request.

Do not place private student information, credentials, complete graded solutions, or confidential SNHU operational information in public GitHub areas.

Internal SNHU routing details should remain in the appropriate internal system.

## When to Escalate

Escalate when:

- the issue is outside the current role's responsibility;
- documented safe troubleshooting does not resolve the problem;
- the supported environment behaves differently from the current course documentation;
- a course-provided artifact appears defective;
- multiple users show the same failure;
- resolving the problem would require privileged or course-maintainer changes; or
- continuing would risk student work, privacy, credentials, or system stability.

Before escalating, collect the evidence described in [Escalation Model](escalation-model.md).

## Related Shared Documentation

- [Course Overview](course-overview.md)
- [Course Repository Architecture](course-repository-architecture.md)
- [Terminology](terminology.md)
- [Supported Environments](supported-environments.md)
- [GitHub Workflow](github-workflow.md)
- [Escalation Model](escalation-model.md)

Return to the [Shared Documentation Index](README.md).
