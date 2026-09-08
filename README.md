# BrainShift

BrainShift chooses a model, reasoning level and speed for each Codex task. Keep using your usual composer; review usage and rate the results in one dashboard.

An independent, experimental app by Jeremi Niedziela. Not affiliated with OpenAI.

## Get the beta

**The next beta is being checked. Downloads are not available yet.** This page will be the starting point for every installation. No particular install order is required.

| Start with | Best for | Beta platform |
| --- | --- | --- |
| Mac app | Codex desktop and a menu-bar dashboard | Apple Silicon, macOS 15 or later |
| Linux app | A dashboard in your browser, opened from the applications menu | Linux x86_64; AlmaLinux 9 build baseline |
| VS Code extension | Codex in VS Code, including Remote-SSH | The same Mac and Linux platforms |

Each native package includes the BrainShift engine; Python is not required. An existing signed-in Codex installation is required for routing. Adding another interface on the same computer reuses your history and settings.

The extension is not yet listed in the Visual Studio Marketplace. Windows, Intel Mac, Linux arm64 and Alpine Linux are not supported by this beta. Linux desktop-client routing remains experimental; the Linux dashboard and VS Code integration are separate features.

## Use it

1. Open BrainShift and review the routing choices in **Settings**.
2. Finish active tasks, then reopen Codex or reload VS Code to connect routing.
3. Submit a task normally. Open the dashboard to inspect the model choice and usage, then rate the result.

Pause routing in the dashboard to keep your selected model for new tasks. For one task, include `\brainshift_skip`; BrainShift removes the command and preserves your selection without asking its advisor.

Use **Install on your devices** to add another interface or a configured SSH host. SSH sign-in must already work; remote extension installation requires an existing VS Code server. Linked devices exchange history and settings when connected. Existing AFS installations need a supervised migration first.

## Usage and privacy

Savings are estimates using recorded tokens and model rates, not a reduction in your subscription bill. Advisor calls also consume usage and appear separately.

Your local history can contain task text and ratings. Routing sends task text and, when needed, recent context to your OpenAI advisor through your existing Codex sign-in. Linked SSH devices exchange execution metadata, task labels, ratings, notes and routing settings; full prompt previews stay on their original installation.

Community sharing is enabled by default, but uploads require individual beta enrolment and access to the collector. Enrolled clients send category, model, rating and usage statistics automatically. They do not upload prompts, titles, notes, task IDs, host names or OpenAI credentials. Turn sharing off in Settings to stop future uploads. Community learning falls back to personal learning when evidence is insufficient.

## Help

[Report a problem](https://github.com/jniedzie/brainshift/issues). Include the BrainShift version, platform, what you expected and what happened. Reports are public: remove private task text and credentials.

BrainShift covers supported native Codex tasks, not ordinary ChatGPT web conversations. Native client updates can affect compatibility. Quitting the dashboard does not disable routing; pause it first. In VS Code, run **BrainShift: Disable Native Routing** before removing the extension. The shared engine and history remain installed.
