# Changelog

All notable changes to the CodeRover desktop app are documented here.

## v0.4.0

**Added**
- GitHub Copilot subscription support with device-flow sign-in, model-catalog synchronization, and Fusion automatic routing.
- Model-specific Copilot API routing for Chat Completions, Responses, and Anthropic Messages.
- Display of Fusion’s selected model.
- Browser tools for navigation, screenshots, clicking, typing, and console inspection.
- Visual image-file reads attached to model conversations.
- Local secrets management with global/workspace scopes, dotenv import, shell environment injection, and tool-result redaction.
- Optional .coderover/environment.yaml configuration for setup commands, environment variables, and named run commands.
- Git tools for commits, branch creation, pushes, PR creation, PR comments, and PR inspection; publishing operations use approval prompts.
- Generic oversized tool-result spilling to per-chat session-state files.

**Improved**
- Delegation guidance for focused sub-agents and independent parallel tasks.
- Settings for Copilot and secrets.
- Copilot credential refresh and model endpoint selection.
- Conversation-summary scheduling and utility-model selection.
- Windows icon visibility

## v0.3.0

- Added persistent shell and richer chat timelines. Shell execution persists across calls, and chat shows clearer tool activity.
- Added Context budgeting: context usage advisor and in-turn compaction.
- Auto model router and the decisions routing client were reworked, and provider/model forms were updated.
- Chat mode persists across new conversations, the scroll-to-bottom button is anchored above the composer, reasoning block spacing is fixed, and timestamps and token usage are shown.
- Tool activity labels and web icons were improved.
- Agent runtime - Turn preparation, finalization, and timeline recording were refactored. Sub-agent runs and edit verification were updated.
- Bug fixes and improvements

## v0.2.0

- Improved chat composer controls
- Added per chat agent todo tracking
- Added per turn Auto model routing using cost and capability tiers.
- Added support 272k Auto context targets and manual Standard/Full budgets
- Added MCP server integration and runtime controls
- Added support for workspace instructions, custom agents, skills, prompts, and hooks
- Added isolated parallel chats with Git worktrees and checkpoint restoration
- Bug fixes and improvements

## v0.1.0

First public release.

- AI coding agent as a native desktop app for **Windows, macOS, and Linux**.
- Local-first: your code and the commands the agent runs stay on your machine.
- Bring-your-own-key - connect Anthropic, OpenAI, any OpenAI-compatible provider, or a local model via Ollama.
- Built-in auto-updates on Windows and macOS.
