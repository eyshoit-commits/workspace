# Agents Configuration & Registration

This document describes how to add, configure, and register agents for OpenCode Manager and compatible plugin systems in this workspace. 

## Purpose
Agents are modular components that provide specific capabilities or automation skills to LLM-based systems. Correct registration and placement of agent files is required for plugins to function.

## General Steps
1. **Fetch the agent package/implementation you want to install.**
2. **Follow the instructions provided in the plugin or agent repository (see below for links/examples).**
3. **Ensure that any required `skills/` or `agents/` folders are copied into the correct location (typically `/bkg/workspace/agents/` or per plugin instructions).**
4. **If the agent must be registered in `opencode.json` or another config, follow the detailed README or installation.md of that plugin.**

## References & Example Repos
- [Oh-My-OpenCode Agent Guide](https://github.com/code-yeongyu/oh-my-opencode/blob/master/docs/guide/installation.md)
- [OpenCode Model Announcer](https://github.com/ramarivera/opencode-model-announcer)
- [Opencode Mem](https://github.com/tickernelz/opencode-mem)
- ... (add more links as you add new agents)

## Best Practices
- Always use the dedicated installer or CLI command if the agent/plugin provides one (e.g. `bunx ... install`).
- Never skip agent/skills copying steps.
- Always confirm agent registration in configuration files.
- Verify after install via CLI/API/health-checks or UI, depending on agent function.

## Agent Example Process with Oh-My-OpenCode

1. Install plugin: `bunx oh-my-opencode install`
2. Answer installation prompts (subscriptions, providers, agent preferences).
3. CLI registers agent and skills (see plugin docs for structure).
4. Check `~/.config/opencode/opencode.json` or project config for agent listing.
5. Authenticate provider if necessary via `opencode auth login` or similar CLI.
6. Test agent with a sample call, plan, or health check.

---

This document should be updated as you add or remove agents from this workspace.

---