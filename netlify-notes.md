## Building CICD Workflow via GitHub Actions

### Terms
CICD -- Continuous Integration and Continuous Delivery

### Notes

#### Building a workflow with a basic step
Entrypoint in Gitlab - /config/yml
GitHub searches the root of the repository (.git)

```shell
# Create .github directory to mark as root
mkdir -p .github/workflows
```

```shell
# Create a yaml workflow
cat hello_world.yaml
```

Upon push, the github action step will be ran
The steps are run sequentially, so the remaining steps will be skipped, should any of the steps fail

In GitLab, the server is mounted automatically
In GitHub, the server needs to be mounted manually

#### Prebuilt-Actions
Pre-built actions are docker containers

Use cases
- Code signing during securities

On Linux, properties in a $ are an environment variable (...)

## Links
[GitHub Actions | Documentation](https://docs.github.com/en/actions/get-started/understand-github-actions)
[GitHub, Run a workflow | Documentation](https://docs.github.com/en/actions/how-tos/manage-workflow-runs/manually-run-a-workflow)
[Cowsays](https://github.com/marketplace/actions/cowsays)