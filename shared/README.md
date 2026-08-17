# Shared IT 140 Support Documentation

The `shared/` directory contains **canonical information that applies to more than one IT 140 support role**.

Support personnel are **not expected to read these pages in order before helping someone**. Role-specific guides should link directly to the shared page or section needed for a particular support task.

> [!IMPORTANT]
> **Shared facts are documented once. Role-specific responsibilities and procedures live under the role's directory.**
>
> When a shared fact changes, update it here and review the role-specific pages that link to it. Do not copy the same fact into multiple role guides unless the role-specific context requires a brief restatement.

## Shared Resources

| Resource | Use It To Understand |
|---|---|
| [Course Overview](course-overview.md) | What IT 140 is, how students work, and which systems provide which kinds of course information |
| [Course Repository Architecture](course-repository-architecture.md) | The purpose of each IT 140 repository and the difference between course templates, student GitHub repositories, and local clones |
| [Terminology](terminology.md) | Common course, environment, GitHub, automation, and support terms |
| [Supported Environments](supported-environments.md) | The CVD reference environment, supported local environments, course IDE components, and unsupported/best-effort configurations |
| [GitHub Workflow](github-workflow.md) | How students create, clone, work in, back up, recover, and reuse course repositories |
| [Support Boundaries](support-boundaries.md) | Which kinds of problems belong primarily to faculty, LSS, advisors, the IT Service Desk, or course technical maintainers |
| [Escalation Model](escalation-model.md) | What evidence to collect and preserve when a problem must move to another support level |

## How Role Guides Should Use Shared Pages

A role-specific page should:

1. Start with the task or decision the supporter needs to make.
2. Include enough context for the supporter to proceed without browsing `shared/` first.
3. Link to the exact shared page or section when a canonical fact is needed.
4. Keep role-specific actions, responsibilities, and escalation instructions in the role directory.
5. Avoid reproducing long explanations that already exist in `shared/`.

For example, a Service Desk procedure for a failed local setup should link to:

- [Supported Environments](supported-environments.md) for the supported-platform facts; and
- [Escalation Model](escalation-model.md) for the evidence package.

The Service Desk procedure should then contain the **Service Desk actions** for that scenario.

## Documentation Ownership

Shared pages should contain facts that remain true regardless of who is helping the student, such as:

- the distinction between D2L Brightspace and GitHub;
- the purpose of a course repository;
- the CVD's role as the course reference environment;
- supported course IDE components;
- repository and Git terminology;
- course automation stages and result language;
- standard diagnostic log locations; and
- the common evidence needed for escalation.

Role-specific directories should contain information such as:

- what that role should do first;
- what that role may or may not change;
- how far that role should troubleshoot;
- what constitutes a successful resolution for that role; and
- where that role sends the problem next.

## Keeping Shared Documentation Current

When course infrastructure changes:

1. Update the authoritative student-facing course or setup documentation first when appropriate.
2. Update the affected shared support page.
3. Search the role guides for links or short restatements that may need revision.
4. Update screenshots if the user interface or expected output changed.
5. Record material support-documentation changes in the repository `CHANGELOG.md`.

Avoid placing rapidly changing artifact versions in general shared pages unless the version itself is needed to explain a support decision. Supporters should use the current course repository and setup instructions when an exact current version matters.

## Screenshots

Screenshots for support documentation belong in:

```text
assets/images/
```

During drafting, use hidden placeholders such as:

```html
<!-- screenshot placeholder; show the relevant verification summary with Result, Failed, and Exit code visible -->
```

A screenshot should clarify a navigation step, expected state, error location, or decision point. Do not add screenshots only for decoration.

## Related Role Guides

- [Faculty Support Guide](../faculty/README.md)
- [LSS Support Guide](../lss/README.md)
- [Advisor Support Guide](../advisors/README.md)
- [Service Desk Triage and Escalation Runbook](../service-desk/README.md)

Return to the [IT 140 Support home page](../README.md).
