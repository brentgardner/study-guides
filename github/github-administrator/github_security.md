# Github Security

- **SECURITY.md** Specifies how to report a secuity vulnerability.
- **Dependabot** alerts will notify you when Github detects a vulnerability a dependeny or malware in the repo.
- **Security Advisories** provide an opportunity to fix and publish information about vulnerabilities. By publishing security advisories, repository maintainers make it easier for their community to update package dependencies and research the consequences of the security vulnerabilities. GitHub stores the published advisories in the Common Vulnerabilities and Exposures (CVE) list. This list is used for automatically notifying affected repositories that use software that has a listed vulnerability.
- **Code Scanning** helps find and triage vulnerabilites and errors in the repo.
- **.GITIGNORE** These files instruct client tools, such as the git command line utility, to ignore paths and patterns when aggregating files for a commit.  If you do check in files that should be ignored, you may use [git-filter-repo](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/removing-sensitive-data-from-a-repository)
- **Branch Protection Rules** enforce certain workflows for one or more branches. For example, you can require an approving review or passing status checks for all pull requests merged into the protected branch.
- **CODEOWNERS** assign individual team members or entire teams as code owners to paths in your repository. These code owners are then required for pull-request reviews on any changes to files in a path for which they're configured.


[More about Github Security Features](https://docs.github.com/code-security/getting-started/github-security-features)

## Documentation

GitHub assigns special significance to these files that makes it easy for collaborators to find them. 

- **README.md**: A README file a guide that provides users with a detailed description of your project.
- **CODE_OF_CONDUCT.md**: A CODE_OF_CONDUCT file defines standards for how to engage in a community.
- **CONTRIBUTING.md**: how to contribute and standards.
- **SECURITY.md**: 
    - A list of supported versions of the project
    - A way to report a security vulnerability.
    - Information about the project's compliance with key privacy and security laws.
    - Technologies that administrators and stakeholders use to secure information.
    - Known risks.


## Securoity Policies

    - Can be defined at both the **organization** and the **enterprise** level. 
        - settings that Enterprise administrators enforce cascade down to all organizations covered by the GitHub Enterprise plan.
        - settings not covered by Enterprise administrators are free to be customized by organization administrators. 
        - Only GitHub Enterprise administrators and organization owners can configure organization security settings. 

## Security Advisories

In the case of a security issue or a vulnerability,  security advisory should be comprehensive and include following information:
- Product and versions affected
- Severity
- Types of security weaknesses addressed by the project owners' actions
- Impact, status of patches, and workarounds

## Repository Rulesets

A named list of rules that apply to a repository.  There is a limit of 75 rulesets per repository.  Anyone with read access to a repo may view rulesets.

Rulesets have the following advantages over branch and tag protection rules:

- Unlike protection rules, multiple rulesets can apply at the same time, so you can be confident that every rule targeting a branch or tag in your repository will be evaluated when someone interacts with that branch or tag.
- Rulesets have statuses, so you can easily manage which rulesets are active in a repository without needing to delete rulesets.
- Anyone with read access to a repository can view the active rulesets for the repository. This means a developer can understand why they have hit a rule, or an auditor can check the security constraints for the repository, without requiring admin access to the repository.

### How they apply

Rulesets are aggrigated at apply time.  If a rule is applied more than one time or in more than one way the most restrictive version wins.  However, all rules are applied.

## Logging

### Standard logs

- available for **90** days
- exportable as **json** or **csv**.

### GraphQL Logs

- available for **120** days

### Rest API

- available for **90** days
