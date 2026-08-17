# IT 140 GitHub Workflow

This page describes the common GitHub workflow used for IT 140 assignments and projects.

It explains the shared workflow rather than replacing the instructions in an activity repository. When supporting a specific assignment or project, follow that repository's current `README.md` for exact commands and files.

## GitHub's Role in IT 140

GitHub is used to:

- host public course repositories;
- create private student assignment and project repositories from course templates;
- maintain remote backups of student work;
- practice Git-based development workflows;
- provide repository Issues, Discussions, and Wikis where appropriate; and
- support course technical documentation and automation.

GitHub is **not** the grading or submission system for normal IT 140 assignments and projects.

D2L Brightspace remains authoritative for:

- activity requirements;
- what to submit;
- grading;
- deadlines; and
- instructor feedback.

## Before Module Two

Course instructions beginning in Module Two assume that the student has:

- access to a GitHub account;
- completed the GitHub account readiness steps in Module One;
- configured two-factor authentication as required by GitHub;
- identified the GitHub username used for IT 140;
- recorded the GitHub-provided `@users.noreply.github.com` email address used for Git configuration; and
- access to a configured course IDE.

For exact account-setup instructions, use the current [`Module One GitHub Account Setup`](https://github.com/GC-STEM/it140-m1-setup-tasks/blob/main/github/README.md).

## The Standard Assignment Workflow

For a new assignment repository, the normal flow is:

```text
Read Brightspace Guidelines and Rubric
              ↓
Read the GC-STEM activity README
              ↓
Confirm the correct GitHub account
              ↓
Create a private student repository from the current template
              ↓
Clone the private repository into ~/Repos
              ↓
Open the local clone in VS Code
              ↓
Complete work
              ↓
Commit and push periodically
              ↓
Submit required deliverables in D2L Brightspace
```

<!-- screenshot placeholder; show a GC-STEM public assignment repository marked as a template and a separate private student repository in the student's GitHub account -->

## Confirm the Correct GitHub Account

The course repositories commonly use GitHub CLI.

A useful first check is:

```bash
gh auth status
```

Confirm that the active account is the GitHub account the student intends to use for IT 140.

When multiple GitHub accounts are configured, the activity README may direct the student to switch accounts.

Do not create a new assignment repository until the correct active account is confirmed.

## Create a Private Repository From the Current Template

The course workflow uses GitHub **templates**, not forks, for student assignment and project repositories.

A typical activity command pattern is:

```bash
cd ~/Repos
gh auth setup-git
gh repo create <repository-name> --template GC-STEM/<repository-name> --private --clone
cd <repository-name>
git remote -v
```

The exact activity README may include additional commands, such as starring the course template.

Use the complete command block from the current activity README rather than reconstructing it from this example.

### Why `git remote -v` Matters

After creation and cloning, `git remote -v` shows which GitHub repository the local copy is connected to.

For normal student work, the local assignment/project repository should point to the **student's private repository**, not directly to the GC-STEM public template.

## Work in the Local Clone

Students normally open the repository folder from:

```text
~/Repos/
```

The repository itself should be the top-level folder shown in the VS Code Explorer.

Examples:

```text
~/Repos/it140-m2-assignment
~/Repos/it140-m3-assignment
~/Repos/it140-m4-assignment
~/Repos/it140-projects
```

The student edits the files identified by the activity README.

Provided READMEs, configuration, tests, SRS/SDD documents, and other course-managed files should remain unchanged unless the activity explicitly permits or requires editing them.

## Commit and Push

Saving a file in VS Code saves it to the local filesystem. It does **not** automatically place the latest work on GitHub.

Students periodically use Git to:

1. review changes;
2. stage the intended files;
3. commit those changes; and
4. push commits to GitHub.

Typical commands include:

```bash
git status
git add <files>
git commit -m "Describe the saved work"
git push
```

Activity READMEs may provide a specific `git add` command that stages only the student working and deliverable files for that activity.

Supporters should prefer the activity-specific command when available.

## Returning to an Existing Assignment

A student normally creates the private repository **once**.

When returning later on the same computer:

1. open VS Code;
2. open the existing repository folder in `~/Repos`; and
3. continue working.

Do **not** create another repository from the template merely because the student is returning to the assignment.

## Moving to Another Computer or a Reset CVD

If the student's private GitHub repository already exists but the local clone does not:

- clone the student's existing private repository;
- do not create another private repository from the course template.

A common pattern is:

```bash
cd ~/Repos
gh repo clone "$(gh api user --jq .login)/<repository-name>"
cd <repository-name>
git status
```

Use the current activity README for the exact command.

## Project Workflow Across Modules Five Through Seven

`it140-projects` is different from the one-module assignment repositories.

The student creates the private `it140-projects` repository **once in Module Five** and continues using the same repository through:

- Module Five / Project One;
- Module Six / Milestone; and
- Module Seven / Project Two.

The student should not create a new `it140-projects` repository for each module.

## Recovering a Damaged Local Copy

If:

- the local folder is damaged, confusing, or incomplete; but
- the student's private GitHub repository contains a good current copy,

the normal recovery model is:

1. preserve or rename the current local folder;
2. clone the existing private GitHub repository again; and
3. verify the new local clone before deleting any backup.

Activity repositories may provide exact **Restore Your Local Copy From GitHub** commands.

> [!CAUTION]
> Never delete the student's only copy of work before confirming that a good copy exists elsewhere.

## Starting Over From the Course Template

Starting over is appropriate only when the student intentionally needs a fresh copy of the current course starting point.

The normal course recovery pattern preserves the previous work by renaming:

- the existing local repository; and
- the existing private GitHub repository,

before creating a new repository from the current template.

This is different from recloning an existing student repository.

Use the activity's current **Start Over From the Original Course Template** instructions when available.

## Repeat Students

Students repeating part or all of IT 140 should create and use repositories from the **current course templates** for the new course attempt.

They should not use an old assignment or project repository as the active working repository for the new attempt.

Using the current template ensures that the student receives the current:

- repository layout;
- instructions;
- starter files;
- tests;
- configuration; and
- support resources.

A prior repository may be preserved under a different name for reference or backup, subject to applicable course and academic-integrity requirements.

## Private Repository Access for Support

A student's assignment or project repository is private.

When an instructor or LSS needs to inspect the repository directly, the student may grant collaborator access when that support workflow is appropriate.

Do not require a student to make a graded-work repository public merely to obtain support.

Role-specific guides should explain when direct repository access is useful and how the supporter should handle student work.

## GitHub Issues and Discussions

Public course repositories may provide:

- **Issues** for technical problems or requested improvements; and
- **Discussions** for repository-related questions or course-community discussion when appropriate.

Do not post in public GitHub areas:

- passwords;
- authentication or verification codes;
- personal access tokens;
- recovery codes;
- private identifying information;
- confidential student information; or
- complete solutions to graded assignments.

Questions about assignment requirements, grading, deadlines, accommodations, and instructor feedback belong through the course/instructor support path rather than a public repository issue.

## Star, Watch, Fork, and Template

These GitHub features serve different purposes:

- **Star** — bookmark a repository so it is easier to find.
- **Watch** — receive repository notifications; generally optional.
- **Fork** — create a linked fork of another repository; not the standard IT 140 student assignment workflow.
- **Use as template / template creation** — create a new independent repository from the course starting point; this is the IT 140 assignment/project model.

## Common GitHub Troubleshooting Questions

Before changing a repository, identify:

```text
GitHub username:
Repository name:
Repository owner:
Repository visibility:
Local path:
Remote URL:
```

Useful commands include:

```bash
gh auth status
git status
git remote -v
```

These checks often reveal whether the problem is:

- the wrong GitHub account;
- the wrong repository owner;
- the wrong local folder;
- a missing local clone;
- a local clone connected to an unexpected remote; or
- a repository that already exists.

## Do Not Use Repository Recreation as the First Fix

A failed command or confusing local folder does not automatically mean the student should start over.

Before recreating a repository:

1. identify the student's existing GitHub repository;
2. determine whether current work has been pushed;
3. determine whether the local clone can be recovered;
4. preserve existing work; and
5. use the activity's documented reset process if a restart is truly needed.

## Related Shared Documentation

- [Course Overview](course-overview.md)
- [Course Repository Architecture](course-repository-architecture.md)
- [Terminology](terminology.md)
- [Supported Environments](supported-environments.md)
- [Support Boundaries](support-boundaries.md)
- [Escalation Model](escalation-model.md)

Return to the [Shared Documentation Index](README.md).
