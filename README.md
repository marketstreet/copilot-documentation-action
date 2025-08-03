# copilot-docs-updater
A Github Action that updates repository documentation every week.

Requires you have access to the Github Copilot Agent, which currently requires a Github Pro+ or Enterprise subscription.

Requires you setup a PAT with the correct permissions and store it in a secret called `GH_ACTION_PAT`; see https://docs.github.com/en/enterprise-cloud@latest/copilot/how-tos/use-copilot-agents/coding-agent/assign-copilot-to-an-issue#creating-and-assigning-a-new-issue

Update the prompt as needed in the action yaml file. Search/replace `your_org_name` and `your_repo_name` with the correct values.
