# IT 140 Terminology

This page defines common terms used throughout IT 140 support documentation.

Use these terms consistently when communicating with students and other supporters. Precise terminology is especially important when a student may have a course template, a private GitHub repository, and a local folder with the same name.

## Course and Instructional Terms

| Term | Meaning in IT 140 |
|---|---|
| **IT 140** | *Introduction to Scripting*, the introductory Python programming course supported by these repositories. |
| **D2L Brightspace** | The course learning-management system. It is the authoritative source for graded activity requirements, submissions, grading, deadlines, and instructor feedback. |
| **zyBooks** | The interactive course textbook and programming-practice environment used for instructional content and labs. |
| **Guidelines and Rubric** | The Brightspace activity page that defines the official requirements, grading criteria, and submission expectations for a graded assignment, milestone, or project. |
| **SDLC** | Software Development Life Cycle. IT 140 repositories use a simplified workflow such as **Analyze → Design → Construct → Test** to organize development work. |
| **SDW** | Software Development Worksheet. A working document used to record analysis or planning notes when provided by an activity. |
| **SRS** | Software Requirements Specification. A document describing what a program or software product is expected to do. |
| **SDD** | Software Design Document. A document describing how a solution is designed. |
| **flowchart** | A visual representation of program logic. IT 140 commonly uses Draw.io `.drawio` files for flowcharts. |
| **pseudocode** | Structured plain-language steps that describe program logic before or without writing the final programming-language syntax. IT 140 uses `.pseudo` files for pseudocode activities. |
| **source code / `src`** | Program code written in a programming language. IT 140 Python source files use the `.py` extension and are commonly stored in `src/`. |
| **tests** | Manual or automated checks used to determine whether a program behaves as expected. Repositories may contain a `tests/` folder even when testing is optional practice for a particular graded activity. |

## Support Roles

| Term | Meaning |
|---|---|
| **Faculty** | Instructors responsible for course instruction, assignment interpretation, grading, instructor feedback, and other faculty responsibilities. |
| **LSS** | **Learning Support Specialist**. The SNHU title used in this repository for personnel who provide learning support to students. |
| **Academic Advisor** | Personnel who support academic planning, course expectations, and referral to appropriate resources. |
| **IT Service Desk** | Personnel who provide technical support and triage for access, devices, supported software, course development environments, and related technical problems within their support scope. |
| **course technical maintainer** | Personnel responsible for maintaining the IT 140 course repositories, automation, course IDE configuration, or related technical artifacts. This is a functional term in this documentation, not an SNHU job title. |
| **supporter** | A general term for any faculty member, LSS, advisor, Service Desk technician, or other authorized person assisting an IT 140 student or colleague. |

See [Support Boundaries](support-boundaries.md) for role-routing guidance.

## Development Environment Terms

| Term | Meaning in IT 140 |
|---|---|
| **IDE** | Integrated development environment. In general computing, this usually refers to software for writing and running code. |
| **course IDE** | IT 140 uses this term broadly for the complete standardized collection of course development tools, settings, extensions, folders, and integrations—not only VS Code. |
| **VS Code** | Visual Studio Code, the primary editor/interface used for IT 140 development work. |
| **Python 3.12** | The Python version targeted by the current supported IT 140 course IDE. |
| **CVD** | Codio Virtual Desktop. The cloud-based Linux desktop used as the IT 140 **reference environment**. |
| **reference environment** | The environment used as the primary course baseline for screenshots, demonstrations, troubleshooting reproduction, and acceptance testing. In IT 140 this is the CVD. |
| **local environment** | A course IDE installed on a student's own supported Windows, macOS, or Linux computer. |
| **supported environment** | A platform for which the course currently provides an approved, documented support path. See [Supported Environments](supported-environments.md). |
| **manual local setup** | A best-effort local installation path for students who do not use the supported automated setup. It is not equivalent to a fully supported course configuration. |
| **terminal** | A text-based window used to enter command-line instructions. Examples include Terminal on Linux/macOS and PowerShell on Windows. |
| **CLI** | Command-line interface. A tool controlled by typed commands rather than primarily through graphical controls. |
| **GUI** | Graphical user interface. A visual application interface using windows, buttons, menus, and other graphical controls. |
| **shell** | The command interpreter running in a terminal. Examples include PowerShell, Bash, and Z shell. |
| **PowerShell** | The primary Windows shell used by the IT 140 Windows automation and supported Windows command examples. |
| **Git Bash** | A Bash-like shell installed with Git for Windows. Some repository instructions support Git Bash, but Windows automation scripts use PowerShell. |
| **home folder / home directory** | The folder associated with the current user account. |
| **`~/`** | A common shorthand for the current user's home folder. It works in the CVD, Linux, macOS, Git Bash, and PowerShell. |
| **`%USERPROFILE%\`** | Windows environment-variable notation for the Windows user-profile folder. It is commonly used in Windows paths such as `%USERPROFILE%\it140\logs\`. |
| **`~/Repos`** | The standard IT 140 workspace folder used for local assignment and project repositories. |
| **`~/it140`** | The standard course automation/configuration folder on CVD, macOS, and Linux. Windows uses the corresponding `it140` folder under the user's profile. |

## Git and GitHub Terms

| Term | Meaning |
|---|---|
| **Git** | Version-control software that tracks changes to files and repository history. Git works locally. |
| **GitHub** | A web-based service that hosts Git repositories and collaboration features. |
| **GitHub CLI / `gh`** | The GitHub command-line tool used in IT 140 for authentication, repository creation, cloning, and other GitHub actions. |
| **repository / repo** | A project folder managed with Git, including its files and version-control history. |
| **course repository** | A public repository maintained by `GC-STEM` that provides course infrastructure, instructions, starter files, or activity templates. |
| **template repository** | A GitHub repository configured so another repository can be created from its current contents without creating a Git fork relationship. |
| **student repository / personal repository** | The private repository in the student's GitHub account created from the current course template for the student's own work. |
| **local repository / local clone** | The repository copy stored in the CVD or on a local computer. This is normally the copy opened and edited in VS Code. |
| **repository root** | The top-level folder of a repository. For example, `~/Repos/it140-projects` is the project repository root. |
| **clone** | Create a local copy of an existing GitHub repository, including Git history and a configured remote. |
| **remote** | A saved connection from a local Git repository to another repository location, usually on GitHub. |
| **`origin`** | The conventional name Git gives to the primary remote when a repository is cloned. |
| **branch** | A line of development in Git. The primary branch in the IT 140 course repositories is generally named `main`. |
| **commit** | A saved snapshot of staged repository changes in Git history. |
| **push** | Send local Git commits to a remote repository such as GitHub. |
| **pull** | Retrieve and integrate changes from a remote Git repository into the current local branch. |
| **fork** | A GitHub copy that retains a fork relationship with another repository. Forking is not the normal IT 140 student assignment workflow. |
| **star** | A GitHub bookmark/favorite. Course instructions may ask students to star a course repository so it is easier to find later. |
| **watch** | A GitHub notification setting for repository activity. Watching is optional unless a course instruction says otherwise. |
| **private repository** | A GitHub repository whose contents are visible only to the owner and explicitly authorized users. Student assignment and project repositories are created as private repositories. |
| **public repository** | A GitHub repository whose contents are publicly visible. GC-STEM course repositories are generally public. |
| **README** | A Markdown file, usually named `README.md`, that explains how to use a repository or folder. IT 140 activity instructions start with the relevant README. |
| **Wiki** | Supplemental repository documentation hosted in GitHub's Wiki feature. Wikis provide background and reference information but do not replace the activity README or Brightspace Guidelines and Rubric. |

See [Course Repository Architecture](course-repository-architecture.md) and [GitHub Workflow](github-workflow.md).

## Course Automation Terms

IT 140 uses a five-stage automation lifecycle:

> **Prepare → Install → Configure → Verify → Update**

| Term | Meaning |
|---|---|
| **Prepare** | Obtains or refreshes the IT 140 course automation package so the approved platform scripts are available. |
| **Install** | Installs or repairs required system-level course software on supported local environments. |
| **Configure** | Configures the current user's course folders, tools, settings, extensions, Git/GitHub integrations, and other course-managed user settings. |
| **Verify** | Checks the current environment and reports its condition **without repairing or changing the course IDE**. Verify is intended to be read-only except for creating its diagnostic log/transcript. |
| **Update** | Maintains approved course IDE software and course-managed assets when directed. It is not a general operating-system upgrade tool. |
| **course automation** | The scripts, manifest, configuration, and supporting files used to prepare and maintain the standardized IT 140 course IDE. |
| **manifest** | A controlled JSON file used by the automation to identify approved software, platforms, sources, settings, and managed assets. |
| **course-managed file** | A script, manifest, schema, setting, or other technical file maintained by the course rather than by the student. Students should not edit these files unless specifically instructed. |
| **artifact version** | A version identifier assigned to a course technical or documentation artifact. Exact current versions may change during course development. |
| **Version DTG** | Version Date-Time Group: a date/time identifier used with some course technical artifacts to distinguish builds or revisions. |
| **log / transcript** | A timestamped text record produced by a lifecycle script. Logs record information such as the script version, platform, actions, and point of failure. |
| **remediation** | A recommended action shown after the automation detects a condition that needs attention. |
| **exit code** | A numeric status returned when a command or script ends. In the IT 140 setup workflow, a normal successful run uses exit code `0`; a nonzero code requires reading the final summary and remediation instructions rather than guessing at a repair. |

## Automation Result Language

| Result | General Meaning |
|---|---|
| **`PASS`** | The lifecycle phase completed successfully. |
| **`FAIL`** | The lifecycle phase encountered a hard failure. Read the final summary and remediation instructions. |
| **`PARTIAL`** | The phase completed only part of its intended work or requires an additional action before it can finish successfully. |
| **`COMPLIANT`** | Verify found the required course environment in an acceptable state. A successful verification reports `Failed: 0` and exit code `0`. |
| **`NOT COMPLIANT`** | Verify found one or more conditions that prevent the environment from meeting the expected course configuration. |
| **warning** | A condition that deserves attention but does not necessarily make the environment noncompliant. Read the associated explanation and recommended action. |
| **failure** | A condition that prevents a check or lifecycle phase from meeting its required result. |

> [!IMPORTANT]
> Do not infer a repair from the result word alone. Read the complete final summary and follow the current remediation or next-step instructions.

## Common File Extensions

| Extension | Typical Use in IT 140 |
|---|---|
| `.py` | Python source code |
| `.md` | Markdown documentation or student text work |
| `.drawio` | Draw.io diagram or flowchart |
| `.pseudo` | Pseudocode |
| `.json` | Structured configuration data, including course automation manifests |
| `.ps1` | Windows PowerShell script |
| `.sh` | Shell script used by Linux-based environments such as the CVD |
| `.zsh` | Z shell script used by the supported macOS automation |

## Preferred Support Wording

Prefer language that identifies the exact object or problem:

- "your **private GitHub repository**" instead of "your GitHub";
- "your **local clone** in `~/Repos`" instead of "your files";
- "the **GC-STEM course template**" instead of "the original repo";
- "the **CVD reference environment**" instead of "Codio" when the desktop environment is specifically meant;
- "the **Verify script**" instead of "the checker";
- "the **final script summary**" instead of "the last error"; and
- "Learning Support Specialist (**LSS**)" as the standard role title.

## Related Shared Documentation

- [Course Overview](course-overview.md)
- [Course Repository Architecture](course-repository-architecture.md)
- [Supported Environments](supported-environments.md)
- [GitHub Workflow](github-workflow.md)
- [Support Boundaries](support-boundaries.md)
- [Escalation Model](escalation-model.md)

Return to the [Shared Documentation Index](README.md).
