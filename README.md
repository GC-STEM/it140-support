# IT 140 Support

This repository is the central support resource for Southern New Hampshire University (SNHU) personnel who support students and faculty in **IT 140 - Introduction to Scripting**.

The repository provides role-specific guidance for:

- [Faculty](faculty/README.md)
- [Learning Support Specialists (LSS)](lss/README.md)
- [Academic Advisors](advisors/README.md)
- [IT Service Desk personnel](service-desk/README.md)

> [!IMPORTANT]
> Start with the guide for **your role**. You are not expected to read the shared documentation first.
>
> Role-specific guides link directly to the shared course information needed to complete each support task.

## Documentation Model

This repository follows one central documentation rule:

> **Shared facts are documented once. Role-specific responsibilities and procedures live under the role's directory.**

Shared documentation provides canonical information about the course, supported environments, terminology, GitHub workflow, support boundaries, and escalation model.

Role-specific documentation:

- explains what a supporter should do;
- links directly to the relevant shared information at the point it is needed;
- avoids requiring supporters to discover or read the `shared/` directory before beginning;
- avoids duplicating shared facts that could become inconsistent over time.

## Choose Your Role

| Role | Start Here | Primary Focus |
| --- | --- | --- |
| Faculty | [Faculty Support Guide](faculty/README.md) | Teaching, student support, course workflow, assignment support, and escalation |
| Learning Support Specialists (LSS) | [LSS Support Guide](lss/README.md) | Student learning support, appropriate code assistance, course tools, and escalation |
| Academic Advisors | [Advisor Support Guide](advisors/README.md) | Course expectations, common student concerns, technology context, and referrals |
| IT Service Desk | [Service Desk Triage and Escalation Runbook](service-desk/README.md) | Technical triage, diagnostics, safe remediation, evidence collection, and escalation |

## Scope

This repository supports the **IT 140 course environment and support workflows**. It is not the authoritative source for graded activity requirements.

For graded assignments and projects:

- **D2L Brightspace** remains the authoritative source for activity requirements, submissions, grading, and instructor feedback.
- Student-facing GitHub repositories provide course tooling, templates, instructions, and supporting resources.
- Support personnel should not provide or publish complete solutions to graded assignments.

## IT 140 Course Repositories

| Purpose | Repository |
| --- | --- |
| Main course hub and course IDE automation | [GC-STEM/it140](https://github.com/GC-STEM/it140) |
| Module One setup tasks | [GC-STEM/it140-m1-setup-tasks](https://github.com/GC-STEM/it140-m1-setup-tasks) |
| Module Two assignment | [GC-STEM/it140-m2-assignment](https://github.com/GC-STEM/it140-m2-assignment) |
| Module Three assignment | [GC-STEM/it140-m3-assignment](https://github.com/GC-STEM/it140-m3-assignment) |
| Module Four assignment | [GC-STEM/it140-m4-assignment](https://github.com/GC-STEM/it140-m4-assignment) |
| Projects One and Two and Module Six Milestone | [GC-STEM/it140-projects](https://github.com/GC-STEM/it140-projects) |

## Repository Structure

```text
it140-support/
├── README.md
├── .github/
│   ├── CHANGELOG.md
│   └── images/
├── shared/
│   ├── README.md
│   ├── course-overview.md
│   ├── course-repository-architecture.md
│   ├── terminology.md
│   ├── supported-environments.md
│   ├── github-workflow.md
│   ├── support-boundaries.md
│   └── escalation-model.md
├── faculty/
│   ├── README.md
│   ├── start-of-term.md
│   ├── setup-and-familiarization.md
│   ├── supporting-students.md
│   ├── assignments-and-grading.md
│   ├── github-and-repositories.md
│   ├── technical-issues-and-escalation.md
│   └── common-scenarios.md
├── lss/
│   ├── README.md
│   ├── orientation-and-familiarization.md
│   ├── workshops-and-office-hours.md
│   ├── learning-support-and-integrity.md
│   ├── github-and-course-tools.md
│   ├── resource-development.md
│   ├── referrals-and-escalation.md
│   └── common-scenarios.md
├── advisors/
│   ├── README.md
│   ├── course-expectations.md
│   ├── technology-context.md
│   ├── student-concerns.md
│   ├── referrals-and-routing.md
│   └── common-scenarios.md
└── service-desk/
    ├── README.md
    ├── triage.md
    ├── environment-troubleshooting.md
    ├── github-repository-troubleshooting.md
    ├── verification-and-logs.md
    ├── safe-remediation.md
    └── escalation.md
```

Role-specific sections intentionally differ in size. A Service Desk runbook requires more technical procedures than an advisor guide; the repository does not force artificial symmetry across roles.

## Shared Documentation

The `shared/` directory contains information that applies to more than one support role.

| Shared Resource | Purpose |
| --- | --- |
| [Shared Documentation Index](shared/README.md) | Index of canonical shared information |
| [Course Overview](shared/course-overview.md) | Course purpose, instructional context, and major technologies |
| [Course Repository Architecture](shared/course-repository-architecture.md) | Purpose and relationship of the IT 140 GitHub repositories |
| [Terminology](shared/terminology.md) | Common IT 140 terms and abbreviations |
| [Supported Environments](shared/supported-environments.md) | Supported course IDE environments and platform expectations |
| [GitHub Workflow](shared/github-workflow.md) | Common GitHub and repository workflow used in IT 140 |
| [Support Boundaries](shared/support-boundaries.md) | Distinguishes technical support, learning support, instructional responsibilities, and advising |
| [Escalation Model](shared/escalation-model.md) | Common escalation principles and evidence expectations |

> [!NOTE]
> These pages are reference sources, not prerequisites. Role-specific documents should link to the exact shared page needed for a procedure.

## Support Principles

Support guidance in this repository should follow these principles:

1. **Start from the supporter's role.** Do not require supporters to learn the repository structure before they can help someone.
2. **Use the supported course workflow.** Avoid generic troubleshooting steps that could move a student farther from the expected IT 140 environment.
3. **Preserve support boundaries.** Technical troubleshooting, learning support, advising, and grading responsibilities are related but not interchangeable.
4. **Collect evidence before escalation.** Escalations should contain enough information for the next support level to continue without restarting the investigation.
5. **Prefer links over duplication.** When a fact is shared across roles, link to the canonical shared page.
6. **Keep instructions current.** Update the canonical source when the course environment or workflow changes.
7. **Protect student privacy and academic integrity.** Do not place sensitive information or complete graded-assignment solutions in public GitHub content.

## Screenshots and Images

Screenshots and other support images should be stored in:

```text
.github/images/
```

Hidden screenshot placeholders may be retained where a future sanitized screenshot would materially improve a procedure. The surrounding text should remain usable without the image, so a placeholder is a maintenance cue rather than a publication blocker.

Example:

```html
<!-- screenshot placeholder; show the IT 140 verification summary with the status and exit code visible -->
```

Do not add screenshots merely for decoration. Screenshots should clarify navigation, expected output, a decision point, or information that a supporter must identify.

## Updating This Repository

Because the IT 140 course environment and support procedures may change rapidly, this repository is intended to be maintained through normal GitHub version-control practices.

When updating documentation:

- change the canonical shared page when a shared fact changes;
- review role-specific pages that link to the changed information;
- avoid copying the revised fact into multiple role guides;
- update procedures when the supported course workflow changes;
- use pull requests for review when practical;
- record material documentation changes in [CHANGELOG.md](./.github/CHANGELOG.md).

## Security, Privacy, and Academic Integrity

Do not post any of the following in public GitHub areas:

- passwords;
- authentication or multi-factor authentication codes;
- GitHub personal access tokens or other access tokens;
- private identifying information;
- confidential SNHU operational information;
- student submissions containing protected information;
- complete solutions to graded IT 140 assignments or projects.

Internal escalation routing, restricted administrative procedures, or security-sensitive information should remain in the appropriate SNHU internal system rather than this repository.

## Development Status

The core support architecture and all four role-specific sections are developed and have completed a cache-busted rendered integration review:

- shared canonical support documentation;
- IT Service Desk triage and escalation runbook;
- faculty support guide;
- LSS support guide; and
- Academic Advisor support guide.

Ongoing maintenance should focus on:

- adding sanitized screenshots only where they materially improve a support procedure;
- keeping restricted routing, queue, contact, and workflow details in the appropriate SNHU internal systems rather than this public repository; and
- updating canonical course facts and linked role procedures as the IT 140 environment evolves.

## Repository Metadata

- **Course**: IT 140 - *Introduction to Scripting*
- **Repository Name**: IT 140 Support
- **Primary Audience**: SNHU faculty, Learning Support Specialists (LSS), academic advisors, and IT Service Desk personnel
- **Repository Purpose**: Provide canonical shared course-support information and role-specific support procedures for IT 140
- **Development Status**: Operational Documentation / Ongoing Maintenance
