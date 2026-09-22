# Hub deployment Skill

Deploy projects on [Hub](https://myhub.host) with your coding agent.

## Get started

In your project, ask your agent:

```text
Follow https://myhub.host/get-started.md and help me deploy this project on Hub.
Verify the deployment and give me its URL.
```

The agent sets up what it needs. Approve sign-in when prompted. It uses hosted MCP for GitHub or the CLI for local files, then checks the release and returns the result.

## Manual installation

```sh
npx skills add Hub-Host/skills --skill hub-deploy
```

Choose your agent in the installer. Installation does not require a Hub account or grant account access. [Connection instructions](https://docs.myhub.host/agents#manual-setup).

[Read the Skill](skills/hub-deploy/SKILL.md) · [Documentation](https://docs.myhub.host)

MIT. See [LICENSE](LICENSE).
