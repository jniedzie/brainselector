# BrainSelector 0.6.60

This release unifies the Mac app, terminal dashboard, VS Code extension, Linux backend, and iPhone companion around the same release and shared data model.

- Capture and route new tasks from ChatGPT desktop, standalone Codex CLI, VS Code, and Claude Code, including queued ChatGPT submissions.
- Restart ChatGPT reliably after delayed Quit, Cancel, and the retained background-process case, with a visible orange action while a restart is needed.
- Discover currently available models dynamically and keep routing choices usable when the catalog changes.
- Keep task history, feedback, community learning, settings, and paired-device state across upgrades.
- Continue showing cached iPhone data when Mac and iPhone versions differ, while suggesting an update instead of blocking the companion.
- Refresh iPhone and widget snapshots promptly, remove rated tasks immediately, and use the same feedback wording across interfaces.
- Show consistent allowance plots and reset timing in the dashboard, terminal, iPhone app, and widget.
- Install or update Mac, Linux, terminal, and VS Code components from one release while preserving the existing data directory and rollback runtime.

The Mac app is Developer ID signed and notarized for Apple Silicon and macOS 15+. Linux is x86_64 with an RHEL 9.8 build baseline. The VS Code Marketplace publishes matching Darwin and Linux packages; the terminal dashboard is included with each native backend.

Finish active tasks before upgrading. Existing history, feedback, settings, pairing identity, and linked-device state are preserved. Checksums accompany every published artifact.
