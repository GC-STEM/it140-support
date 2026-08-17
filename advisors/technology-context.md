# IT 140 Advisors | Technology Context

This page explains the IT 140 technology environment at the level an advisor needs to recognize student concerns and route them correctly.

You do **not** need to troubleshoot these tools.

## The Most Important Technology Fact

> **A student does not need to successfully install the IT 140 course IDE on a personal computer in order to complete the course when the CVD is available and working.**

The **Codio Virtual Desktop (CVD)** is the IT 140 reference environment.

It provides a cloud-based desktop that students access through a web browser.

This means a local-computer setup problem does not automatically mean the student cannot continue coursework.

<!-- screenshot placeholder; show the student-facing CVD desktop in a browser with VS Code visible, emphasizing that the programming environment runs in the browser -->

## Codio Virtual Desktop (CVD)

At a high level:

- the CVD is accessed through the course/Codio path;
- it provides the course development tools in a managed virtual environment;
- students use it to write and run Python code;
- it is the reference environment for course screenshots and troubleshooting; and
- it can provide continuity when a supported local installation is unavailable.

If the student cannot access or launch the CVD, that is a **technical-support problem**.

## Supported Local Computers

Students may optionally configure the course IDE on a supported Windows, macOS, or Linux computer.

Exact supported operating-system versions and setup procedures can change.

Advisors should **not** memorize or communicate specific version requirements from memory.

Use [Supported Environments](../shared/supported-environments.md) or the current
[Module One Setup Tasks](https://github.com/GC-STEM/it140-m1-setup-tasks) when exact platform support matters.

## Chromebooks, Tablets, and Other Devices

A device that cannot run the supported local course IDE may still be usable to **access the CVD through a supported web browser**.

Therefore:

- do not conclude that a student must purchase a new computer solely because local setup is unsupported;
- do not promise that every device/browser configuration will work; and
- route access/device-specific problems to the IT Service Desk.

The Service Desk can determine whether the student's device and access path are functioning appropriately.

## VS Code

**Visual Studio Code (VS Code)** is the primary editor/interface students use for course development.

Students may say:

- "VS Code is broken";
- "my code won't run";
- "Python isn't working"; or
- "the terminal doesn't work."

Those statements need classification.

### If VS Code or Python Cannot Function

Examples:

- VS Code will not launch;
- Python cannot run at all;
- required course tools are missing;
- the configured environment fails Verify.

**Route:** IT Service Desk.

### If VS Code Works but the Student's Code Is Wrong

Examples:

- Python runs but gives unexpected output;
- the student has a syntax error;
- the student does not understand a loop or function.

**Route:** faculty or LSS.

## GitHub

Students may describe GitHub as "where my assignment is."

A simpler advisor mental model is:

> **GitHub stores the student's course-development repository; D2L Brightspace receives the graded submission.**

Students may use GitHub to:

- create a private assignment/project repository from a course template;
- maintain a remote copy of their work; and
- restore their work when moving to another supported environment.

Advisors do not need to know Git commands or repository-recovery procedures.

### Route GitHub Problems by Type

| Student Concern | Route |
| --- | --- |
| "I don't understand why we use GitHub." | Faculty or LSS can explain the learning/course workflow |
| "I can't sign into GitHub." | IT Service Desk |
| "The command to create/clone my repo fails." | IT Service Desk |
| "I can't find my files after changing computers." | IT Service Desk for repository recovery |
| "Do I submit the GitHub link?" | Current D2L Guidelines and Rubric / faculty |

## Technical Problems Can Sound Academic

A student may say:

> "I can't do the assignment."

Before assuming the student cannot understand the material, ask a simple routing question:

> "Is the problem that the course tools will not work, or that the programming itself is confusing?"

The answer often identifies the correct next resource without technical troubleshooting.

## Do Not Recommend Generic Technical Fixes

Advisors should not direct students to:

- uninstall/reinstall Python;
- delete repositories;
- reset the CVD;
- change Git configuration;
- disable security software;
- run administrator/root commands; or
- install random versions of course software.

Technical repair belongs to the IT Service Desk and current course procedures.

Return to the [Advisor Support Guide](README.md).
