# BrainShift

Adaptive model routing for Codex, by Jeremi Niedziela.

## Download the beta

- [Mac app — Apple Silicon](https://github.com/jniedzie/brainshift-feedback/releases/latest/download/BrainShift-macOS-arm64.zip)
- [VS Code extension](https://github.com/jniedzie/brainshift-feedback/releases/latest/download/brainshift.vsix)
- [Release notes and checksums](https://github.com/jniedzie/brainshift-feedback/releases/latest)

Mac: unzip, drag **BrainShift.app** into Applications, and open it. Python 3 is required. This beta is not yet Developer ID signed or notarized; macOS may require **System Settings → Privacy & Security → Open Anyway** after attempting to open it.

VS Code: run **Extensions: Install from VSIX…**, select the file, then reload. Use **BrainShift: Enable Native Routing** to enable interception for new Codex sessions. Expand **Install on your devices** in either dashboard to install the companion or deploy to a configured SSH host.

Add `\brainshift_skip` anywhere in a task to keep your selected model. The command is removed before submission.

## Feedback

[Send feedback](https://github.com/jniedzie/brainshift-feedback/issues/new). Include the version, platform, and expected and actual behavior. Issues are public: exclude credentials and private prompts.

## Beta scope

This experimental integration supports native Codex desktop and VS Code workflows, not ordinary ChatGPT web chats. Routing uses an advisor and can make mistakes. You retain an off switch and per-prompt skip command. Credit savings compare recorded tokens at original and chosen model rates, not an alternative execution. Monetary values are illustrative scenarios, not bill savings.

The code repository is private; runtime downloads necessarily contain executable implementation files. No personal usage database, prompts, credentials, or developer configuration is included. Community feedback collection is not connected; no aggregate data is transmitted yet.
