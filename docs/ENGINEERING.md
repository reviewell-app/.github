# Reviewell — engineering handbook

This is shared guidance for changes across the organisation. A repository's own instructions take precedence. These expectations are a delivery checklist, not a claim that every existing project has implemented every item.

## Start a change

State the user problem, the intended result and the smallest useful scope. Check existing issues and project instructions. For a substantial change, discuss the approach before implementation.

## Keep the work reviewable

- Make focused commits and pull requests with a clear problem and result.
- Follow the existing architecture and conventions unless the change requires otherwise.
- Explain changes to data, permissions, configuration and external integrations.
- Include a practical before-and-after example when behaviour changes.

## Validate what matters

Run the checks documented by the project. Test the affected user path and meaningful failure cases. For interface changes, check keyboard navigation, focus, empty states, loading, errors and relevant screen sizes. Respect reduced-motion preferences.

Use synthetic data and redact logs. Report what was actually verified, including anything that could not be checked; do not describe an attempted test as a passing one.

## Prepare a release

1. Confirm the intended version and product maturity: experiment, preview or release.
2. Document installation, platform requirements and required permissions.
3. Describe configuration or migration steps and retain a recovery path where relevant.
4. Write release notes around changes that matter to the user.
5. Check download, support and documentation links before publishing.

Project-specific signing, distribution, deployment and rollback instructions remain in the product repository.

## Handle information deliberately

Keep secrets outside source control. Use only the information a feature needs, explain permissions and avoid putting customer data in issues or screenshots. Changes involving authentication, access control, billing or destructive actions need explicit review of the affected path.

Use the [security reporting instructions](../SECURITY.md) for suspected vulnerabilities.

## Maintain the public profile

The organisation start page lives in `profile/README.md`; its visual assets live in `assets/`. Product links should point to the current authoritative home. Do not list unreleased private projects or make performance, customer or release claims without supporting evidence.

Keep the page readable with images disabled. Use descriptive links and image alternatives, and preview changes on GitHub after publication.
