# Repository security and management
You can oversee the security and management of your repositories in several ways.

## Create protection rules

To manage changes to content within your repository, you can create branch protection rules to enforce certain workflows for one or more branches. Protection rules that can be applied to a branch include:
- Require a pull request before merging.
- Require status checks to pass before merging.
- Require conversation resolution before merging.
- Require signed commits.
- Require linear history.
- Require merge queue.
- Require deployments to succeed before merging.
- Lock the branch by making it read-only.
- Restrict who can push to matching branches.
- Additionally, you can set branch rules that apply to everyone, including administrators. For example, you can allow force pushes to matching branches and allow deletions from users who have push access.
- Add a `CODEOWNERS` file

By adding a `CODEOWNERS` file to your repository, you can assign team members or entire teams as code owners who are responsible for code in the repository. When someone opens a pull request that modifies code that belongs to a code owner, the code owner is automatically requested as a reviewer.
You can create the `CODEOWNERS` file in either the root of the repository or in the docs or .github folder.

## View traffic by using Insights

Anyone who has push access to a repository can view its traffic. In the traffic graph, they can view full clones (not fetches), visitors from the past 14 days, referring sites, and popular content.