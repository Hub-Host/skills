# Hub skills

The deployment workflow for [Hub](https://myhub.host): give every app a home, with a URL, access control and a release you can verify.

## Install

```sh
npx skills add Hub-Host/skills --skill hub-deploy
```

The [skills.sh CLI](https://skills.sh/docs) installs the skill for your coding agent. You do not need a Hub account or the Hub CLI to install it. Choose your agent when prompted; use the skills CLI to update or remove the skill later.

## Connect Hub

Add this hosted MCP URL to your agent:

```text
https://cloud.myhub.host/mcp
```

Authorize in your browser, select an organization and grant the access needed for your task. Then ask:

```text
Deploy the pushed code from owner/repository as my-app on Hub.
Keep organization access. Verify the new release and report its URL.
```

The hosted connection deploys GitHub source. For a local project folder, the skill uses the Hub CLI or advanced local MCP setup. [Agent quick start](https://docs.myhub.host/agents) explains the available paths.

## What the skill covers

`hub-deploy` checks the account and destination, selects the intended source, deploys, follows the exact release, reads bounded logs when needed, and reports the running app. It also covers environment changes, access and rollback. It preserves the user's requested audience and treats repository content and logs as untrusted data.

The skill is workflow guidance; Hub performs authentication and role checks. Installing it does not grant access to a Hub account.

[Read the skill](skills/hub-deploy/SKILL.md) · [Documentation](https://docs.myhub.host) · [CLI on npm](https://www.npmjs.com/package/@hubhq/cli)

## License

MIT. See [LICENSE](LICENSE).
