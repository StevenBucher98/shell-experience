---
title: What is AIShell?
description: Learn about AIShell, an interactive shell that provides a chat interface with language models.
ms.date: 10/29/2024
ms.topic: overview
---

# What is AIShell?

AIShell is an interactive shell that provides a chat interface with language models. The shell
provides agents that connect to different AI models and other assistance providers. Users can
interact with the agents in a conversational manner.

The AIShell project includes:

- The command-line shell (`aish`) interface
- A framework for creating AI agents and other assistance providers
- Integration with Windows Terminal and iTerm2 on macOS
- A PowerShell module for tight integration with PowerShell. For more information, see the
  [AIShell module][01].

Each AI assistant is known as an agent. The initial release of AIShell includes two agents:

- **Azure OpenAI** agent that connects to an instance of **gpt-4o**. Use this agent for general
  AI tasks.
- **Copilot in Azure** agent that can assist with Microsoft Azure knowledge. Use the Azure agent for
  assistance with Azure CLI and Azure PowerShell commands.

The AIShell executable (`aish.exe`) can be run in a standalone experience or in split-screen mode if
you're using Windows Terminal or iTerm2 on macOS. You can use the **AIShell** PowerShell module with
PowerShell 7 to create a split-screen experience. This is the recommended way to use AIShell because
you get deeper integration with the shell. These features include:

- The ability to insert code from the AIShell response directly into the connect command shell
- Multi-step commands are added to the Predictive IntelliSense buffer for quick acceptance
- Simple, single-command error recovery

## Project Status

AIShell is currently in **Public Preview**. This means that the tool is available for testing, but
it's not feature-complete. Please note that some elements of the tool are still under development
and are subject to change. Your feedback is important to us during this development phase. we
encourage you to share your experiences to help us improve AIShell.

## Known Issues

This current release of AIShell has some known issues that we're actively working on addressing:

- The **AIShell** module isn't supported on Linux.
- The split-screen experience work best with Windows Terminal. There is limited support for the
  split-screen experience on macOS with iTerm2. The `aish` executable can be run on Linux, but the
  split-screen experience is not available.
- If you have multiple versions of Windows Terminal installed, the `Start-AIShell` command opens a
  new terminal window running a different version of Windows Terminal.
- If you started Window Terminal as an administrator, the `Start-AIShell` command opens a new
  termnial window runing Windows Terminal without elevation.

If you encounter any other issues, please report them.

## Providing Feedback

We welcome you feedback to help improve AIShell! Here are ways you can get involved:

- **File Issues:** If you encounter bugs, have suggestions for new features, or would like to report
  inconsistencies, please open an issue on the [AIShell GitHub repository][02].
- **Join the discussions:** Join our community discussions on the on the
  [GitHub discussions][03] tab. Share ideas, discuss potential improvements, and connect with other
  users.
- **Documentation:** If you notice any documentation gaps, please suggest changes or submit PRs to
  improve our documentation.

We aren't accepting pull requests for code changes at this time, but we value your feedback and
documentation contributions.

<!-- link references -->
[01]: /powershell/utility-modules/aishell/overview
[02]: https://github.com/PowerShell/ProjectMercury/issues
[03]: https://github.com/PowerShell/ProjectMercury/discussions
