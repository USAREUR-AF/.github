# USAREUR-AF/.github

Shared defaults for every public repository in the USAREUR-AF organization.

GitHub uses the issue templates and the pull request template in this repository for any repository that doesn't have its own. A repository that needs something different, such as goatcore, keeps its own copy, and that copy wins.

- `.github/ISSUE_TEMPLATE/`: bug report, feature request, and the links for security reports and questions.
- `.github/PULL_REQUEST_TEMPLATE.md`: the pull request checklist.

Changes here affect every repository without its own templates, so keep them short and general. The project standards are tracked in [goatcore#103](https://github.com/USAREUR-AF/goatcore/issues/103) and the issues it links.

## Reporting a vulnerability

Report against the affected repository. Open that repository's **Security** tab, select **Advisories**, and choose **Report a vulnerability**. Read its `SECURITY.md` for any additional instructions. If that button is unavailable, follow the private contact route in that repository's security policy. Do not post vulnerability details in a public issue or Discussion.

A report is private to the people GitHub grants access to the advisory, including maintainers and explicitly added collaborators. A CODEOWNERS entry alone does not define advisory access.

## Maintaining the templates

GitHub uses the whole issue-template folder from a repository when that repository has its own issue template or configuration. It does not combine that folder with these defaults. PR-template overrides are independent. See [GitHub's default community-health file documentation](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file).

The labels `bug`, `enhancement` and `needs-triage` must exist in this repository and in repositories using these forms. After changing a form, open the issue chooser in a repository without local templates and verify both forms and the security link. CI in this repository checks contributions to these defaults; workflows themselves are not inherited by other repositories.
