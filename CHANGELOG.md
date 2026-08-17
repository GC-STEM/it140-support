# Changelog

All notable documentation and structural changes to the IT 140 Support repository should be recorded in this file.

## Unreleased
### Added
- Initial `it140-support` repository architecture.
- Top-level repository purpose, scope, support principles, and role-based navigation.
- Shared-documentation directory and placeholder outlines.
- Role-specific directories for faculty, Learning Support Specialists (LSS), academic advisors, and IT Service Desk personnel.
- `assets/images/` directory for screenshots and other support images.
- Documentation convention requiring role-specific guides to link directly to relevant shared information.
- Hidden screenshot-placeholder convention for documentation under development.
- Developed the IT Service Desk triage and escalation runbook with role-specific procedures for triage, supported environments, GitHub/repositories, verification/logs, safe remediation, and escalation.
- Developed the faculty support guide with start-of-term reorientation, faculty setup/familiarization, student support, assignment/grading, repository, escalation, and common-scenario guidance for adjunct faculty.
- Developed the LSS support guide with role orientation, Python Workshop and IT Basic Office Hours guidance, learning-support and academic-integrity practices, course-tool/repository guidance, Academic Resource Center development, referral/escalation, and common-scenario guidance.

### Changed

- Refactored `shared/course-repository-architecture.md` so repository recovery and repeat-student procedures are canonical in `shared/github-workflow.md` rather than duplicated in the architecture page.
- Refined Service Desk remediation and escalation pages so lifecycle definitions, platform facts, and the common evidence schema remain canonical in `shared/`, while Service Desk pages retain role-specific actions.
- Added explicit return-to-runbook navigation to Service Desk procedure pages.
