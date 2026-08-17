# IT 140 Faculty | Supporting Students

Faculty support spans assignment interpretation and programming instruction, but IT 140 also has dedicated technical and learning-support paths.

Use this page to identify **what kind of help the student needs before deciding what to do next**.

## Start With the Student's Goal

Ask what the student is trying to do and identify the failing layer.

Common categories are:

| Student Problem | Primary Path |
| --- | --- |
| Cannot access Brightspace, Codio, GitHub account, or supported course tool | Technical / IT Service Desk |
| Course IDE will not configure or Verify | Technical / IT Service Desk |
| Cannot create, clone, or find the expected repository | Repository workflow; faculty may orient, Service Desk handles technical failures |
| Does not understand assignment requirements | Faculty |
| Does not understand a programming concept | Faculty or LSS |
| Python runs but student code has a syntax/logic problem | Faculty or LSS |
| Wants grading clarification or feedback interpretation | Faculty |
| Needs academic planning advice | Academic Advisor |

See [Support Boundaries](../shared/support-boundaries.md) for the canonical role definitions.

## For Assignment Questions

Start with the **current D2L Brightspace Guidelines and Rubric**.

Use the activity repository README to understand:

- the development workflow;
- provided starter files;
- file/folder locations;
- optional practice or tests;
- repository-specific help; and
- how the student is expected to work with the course tooling.

If the repository appears to contradict the current Guidelines and Rubric, do not silently reinterpret the graded requirement. Use Brightspace for grading and report the documentation conflict.

## For Student-Code Questions

If Python and the course environment work but the student's own program fails:

- help the student identify the specific error or unexpected result;
- ask what the student expected the program to do;
- connect the problem to concepts the student has learned;
- encourage small tests and incremental debugging;
- use hints, questions, or partial examples before supplying a complete solution; and
- refer to LSS when additional learning support would help.

The goal is to help the student develop and debug **their own solution**.

Do not route a normal student syntax or logic error to the Service Desk merely because the error appears in VS Code or Terminal.

## For Technical Environment Problems

Faculty do not need to perform deep system troubleshooting.

If the problem appears environmental:

1. identify whether the student is using CVD, Windows, macOS, Linux, or an unsupported environment;
2. confirm whether the CVD is available as a continuity path;
3. preserve the exact error or Verify summary when practical; and
4. refer the student through the technical support path.

The [Service Desk Triage](../service-desk/triage.md) shows the technical classification model.

> [!TIP]
> If a local setup problem is consuming the student's course time, encourage the student to continue working in the CVD while the local issue is investigated.

## For Repository Problems

First distinguish:

- GC-STEM public course template;
- student's private GitHub repository; and
- student's local clone.

See the [Three-Copy Model](../shared/course-repository-architecture.md#the-three-copy-model).

Faculty can often help a student recognize that they opened the wrong copy or are looking in the wrong folder without changing Git state.

For technical authentication, remote, clone, or recovery problems, use the Service Desk/repository support path rather than improvising destructive Git commands.

## Protect Student Work

Do not use deletion or recreation as the first troubleshooting step.

Before anyone resets or replaces a student repository:

- determine whether the student's current work exists on GitHub;
- preserve local-only work;
- avoid deleting Git history; and
- use the current activity recovery/start-over process.

See [GitHub Workflow](../shared/github-workflow.md).

## Public Support Channels

Do not ask students to post:

- passwords or authentication codes;
- access tokens;
- private identifying information;
- private repository contents; or
- complete graded solutions

in public GitHub Issues or Discussions.

A public course question can often be asked without including the student's private work.

## When to Refer to LSS

LSS is appropriate when a student would benefit from additional help with:

- programming concepts;
- pseudocode or flowchart reasoning;
- debugging strategy;
- testing;
- reading error messages; or
- developing problem-solving habits.

Faculty retain authority for assignment interpretation, grading, and instructor feedback.

## When to Refer to the Service Desk

Use the technical path when the primary issue is:

- account/system access;
- CVD launch or configuration;
- supported local course IDE installation/configuration;
- GitHub authentication;
- GitHub CLI failure;
- repository creation/clone failure;
- Verify failure; or
- another supported technical environment problem.

For faculty-specific handoff guidance, see [Technical Issues and Escalation](technical-issues-and-escalation.md).

Return to the [Faculty Support Guide](README.md).
