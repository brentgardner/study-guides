# Github Actions

## Enterprise Level

- Github Actions Use Policy: configuring a use policy for workflows and actions in your enterprise is essential to prevent users from using malicious third-party actions.

| GitHub-hosted runners	 | Self-hosted runners |
| ---------------------- | ------------------- |
| Receive automatic updates for the operating system, preinstalled packages and tools, and the self-hosted runner application. |	Receive automatic updates for the self-hosted runner application only. You're responsible for updating the operating system and all other software. |
| GitHub managed and maintained. |	Can use cloud services or local machines that you already pay for. Also are customizable to your hardware, operating system, software, and security requirements. |
| Provide a clean instance for every job execution.	 | Don't need to have a clean instance for every job execution. |
| Use free minutes on your GitHub plan, with per-minute rates applied after surpassing the free minutes. |	Are free to use with GitHub Actions, but you're responsible for the cost of maintaining your runner machines. |

### Labels

Self-hosted runners automatically receive default labels when they're added to GitHub Actions. These default labels indicate the operating system and hardware architecture of the runner as shown in the table:

| Default Label | Description |
| ------------- | ----------- |
| `self-hosted` | Default label applied to all self-hosted runners |
| `linux`, `windows`, or `macOS` | Applied depending on the runner's operating system. |
| `x64` , `ARM`, or `ARM64` | Applied depending on the runner's hardware architecture.

Also supports custom labels.

### Troubleshooting runners

| Mac	| Windows	| Linux |
| ----- | --------- | ----- |
| Check the self-hosted runner application service using `launchd` | Check the self-hosted runner application service using `PowerShell` | Check the self-hosted runner application service using `journalctl` If your jobs require containers, check that Docker is installed and running and the Docker permissions using systemctl |


## Organization Level

## Github Packages

GitHub Packages allow you to share your project dependencies within your organization or publicly.  You may use a single set of credentilals to support packages in many package managers.

Compatable with common package managers such as:

- NPM (NodeJS)
- NuGet (.NET)
- RubyGems (Ruby)
- Maven & Gradle (Java)

URLS: PACKAGE-REGISTRY.pkg.github.com.

### Github Packages vs Github Releases

GitHub Packages are used to publish releases of your libraries to a standard package feed or a container registry. They are meant to leverage the ways the specific package-management client works with that feed, like linking back to the repository in which the package was created as well as the version of the code that was used.

GitHub Releases are used to release a bundle of packaged software, along with release notes and links to binary files. You can download those releases directly from their unique URL and track them back to the specific commit they were created from. You can only download releases as tarballs or ZIP files.

### Authenticate to GitHub Packages
The way you authenticate into your package manager will depend on your project's ecosystem. Whichever ecosystem you're working with, you'll need three pieces of information:
- Your GitHub username
- A Personal Access Token
- The GitHub Packages endpoint for your package ecosystem

### Container Registry

Github Packages is also a contrainer registry. You can use GitHub Container Registry to seamlessly host and manage Docker container images in your GitHub organization or personal user account

With the container registry, you can:
- Store container images within your organization and user account rather than a repository.
- Set fine-grained permissions for the container images.
- Access public container images anonymously.

URLs: ghcr.io/OWNER/IMAGE-NAME