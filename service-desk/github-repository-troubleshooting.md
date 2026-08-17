# IT 140 GitHub and Repository Troubleshooting

Use this page for GitHub authentication, repository creation, cloning, remote, and repository-location problems.

Before changing anything, understand the
[Three-Copy Model](../shared/course-repository-architecture.md#the-three-copy-model):

```text
GC-STEM public course template
          ↓ create from template
Student's private GitHub repository
          ↓ clone
Student's local repository in ~/Repos
```

## First: Identify the Exact Repository

Collect:

```text
GitHub username:
Repository name:
Repository owner:
Repository visibility:
GitHub repository URL:
Local repository path:
```

From the local repository root, run:

```bash
git status
git remote -v
```

The normal student assignment/project local clone should point to the student's private GitHub repository, not directly to `GC-STEM`.

<!-- screenshot placeholder; show GitHub repository breadcrumbs for a GC-STEM public template and a student private repository, emphasizing the different owner names -->

## GitHub Authentication

From a Terminal/PowerShell window, run:

```bash
gh auth status
```

Confirm the active GitHub account is the account the student intends to use for IT 140.

If authentication is missing or the wrong account is active, use the current course setup/configuration workflow rather than collecting the student's password or token.

> [!WARNING]
> Never ask the student to send a GitHub password, device code, two-factor authentication code, recovery code, passkey, personal access token, or other credential.

## Repository Already Exists

An "already exists" message is usually a **state-identification problem**, not a reason to delete the repository immediately.

Determine whether:

- the student's private GitHub repository already exists;
- the local folder already exists;
- both exist and are connected correctly; or
- one copy is missing.

Use the canonical recovery paths in
[GitHub Workflow](../shared/github-workflow.md#returning-to-an-existing-assignment).

## Local Folder Missing, GitHub Repository Exists

If the student's private GitHub repository contains the current work but the local clone is missing, clone the **existing private repository**.

Do not create a second repository from the public course template merely because the local folder is absent.

See [Moving to Another Computer or a Reset CVD](../shared/github-workflow.md#moving-to-another-computer-or-a-reset-cvd).

## Local Clone Damaged, GitHub Copy Is Good

Preserve or rename the existing local folder before recloning the student's existing private repository.

Do not delete the old local copy until the replacement clone has been verified.

See [Recovering a Damaged Local Copy](../shared/github-workflow.md#recovering-a-damaged-local-copy).

## Student Cloned the GC-STEM Template Directly

A direct clone of `GC-STEM/it140-mX-...` is not the normal student assignment workflow.

Before replacing it:

1. Check whether the student has added work to the direct clone.
2. Preserve that work.
3. Use the activity README to create the student's private repository from the current template.
4. Move/copy only the appropriate student work into the correct private-repository workflow as directed by the activity/support process.

Do not push student work into the public GC-STEM repository.

## Wrong Remote

If `git remote -v` points somewhere unexpected, stop before pushing.

Record the output and determine which repository should be `origin`.

Do not rewrite remotes blindly when the student's current work or Git history has not been assessed.

## Projects Repository Across Modules Five Through Seven

Students create `it140-projects` **once in Module Five** and continue using that same private repository for Modules Five, Six, and Seven.

Creating separate project repositories for each of those modules is not the intended workflow.

See [Projects | Modules Five Through Seven](../shared/course-repository-architecture.md#projects--modules-five-through-seven).

## Repeat Students

A student repeating part or all of IT 140 should use a repository created from the **current course template** for the new course attempt rather than using an old assignment/project repository as the active repository.

See [Repeat Students](../shared/github-workflow.md#repeat-students).

## Starting Over

Starting over from the current course template is different from restoring the student's existing GitHub repository.

Before starting over:

- preserve local work;
- preserve/rename the existing private GitHub repository;
- use the activity's current reset/start-over instructions; and
- do not delete the only copy of student work.

See [Starting Over From the Course Template](../shared/github-workflow.md#starting-over-from-the-course-template).

## When the Public Course Repository Looks Wrong

If a current GC-STEM repository is missing, unavailable, or appears defective:

1. Check [Course Status](https://github.com/GC-STEM/it140/wiki/Course-Status).
2. Confirm the current activity README/URL from Brightspace or the main course repository.
3. Reproduce the problem without using private student data when possible.
4. Escalate through [Course Technical Maintenance Escalation](escalation.md#course-technical-maintenance-escalation).

Do not create a workaround that permanently diverges the student's repository from the current course template unless course support directs it.
