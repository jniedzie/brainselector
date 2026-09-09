# BrainSelector

BrainSelector chooses a model, reasoning level and speed for each Codex task.

## Prerequisites

A working installation of the ChatGPT app and/or the VS Code Codex extension is needed.

## Get the beta

The app is available for Mac, Linux, and as a VS Code extension. You can install just one of them, then the dashboard will allow you to install the other ones if needed.
Adding another interface on the same computer reuses your history and settings.

| Start with | Best for | Beta platform |
| --- | --- | --- |
| [Mac app](https://github.com/jniedzie/brainselector/releases/download/v0.6.4/BrainSelector-0.6.4-macOS-arm64.dmg) | ChatGPT desktop app with a menu-bar dashboard | Apple Silicon, macOS 15 or later |
| [Linux app](https://github.com/jniedzie/brainselector/releases/download/v0.6.4/BrainSelector-0.6.4-Linux-x86_64.tar.gz) | A dashboard in your browser, opened from the applications menu | Linux x86_64; AlmaLinux 9 build baseline |
| [VS Code extension](https://marketplace.visualstudio.com/items?itemName=jniedzie.brainselector) | Codex in VS Code, including Remote-SSH | The same Mac and Linux platforms |

[Download the latest beta and view checksums](https://github.com/jniedzie/brainselector/releases).

On Mac, open the downloaded disk image and drag BrainSelector to Applications.

The Linux desktop-client routing is very experimental (=untested).

## Use it

After the app/extension is installed and running, restart your ChatGPT app and VS Code. 
Now you can just send your prompts as usual and the magic will happen automatically (even though you may not see the model changing in the UI).

To see more details:
1. Open BrainSelector using the brain icon in the macOS manu-bar or in the VS Code Codex extension window.
2. Have a look at all the stats in the dashboard.
3. Check the **Settings** section for more control over BrainSelector.
4. Review recent rerouting decisions - select your rating for each tast, optionally provide a comment, then save it.

You can pause routing in the dashboard to keep your selected model for new tasks. For one task, include `\skip` - it will be removed from the prompt and preserve your model selection for that prompt. Code examples and longer names are left unchanged. The previous commands still work.

Use **Install on your devices** to add another interface or install the extension on a configured SSH host. SSH sign-in must already work; remote extension installation requires an existing VS Code server. Linked devices exchange history and settings when connected.

## Usage and privacy

Savings are estimates using recorded tokens and model rates, but not your actual bill - take it with a large grain of salt. Advisor calls also consume usage and appear separately.

Your local history contains task text and ratings. Routing sends task text and, when needed, recent context to your OpenAI advisor through your existing Codex sign-in. Linked SSH devices exchange execution metadata, task labels, ratings, notes and routing settings; full prompts stay on their original installation.

Community sharing is enabled by default. Clients send category, model, rating and usage statistics automatically. They do not upload prompts, titles, notes, task IDs, host names or OpenAI credentials. Turn sharing off in Settings to stop future uploads.

## Help

[Report a problem](https://github.com/jniedzie/brainselector/issues). Include the BrainSelector version, platform, what you expected and what happened. Reports are public: remove private task text and credentials.

BrainSelector covers supported native Codex tasks, not ordinary ChatGPT web conversations. Native client updates can affect compatibility. Quitting the dashboard does not disable routing; pause it first. In VS Code, run **BrainSelector: Disable Native Routing** before removing the extension. The shared engine and history remain installed.
