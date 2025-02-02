---
title: Install AIShell
description: Learn how to install AIShell on your system.
ms.date: 10/29/2024
ms.topic: install-set-up-deploy
---
# Install AIShell

AIShell is an interactive shell that provides a chat interface with language models. There are
packages you need to install to have a complete AIShell experience.

- The command-line shell (`aish`) interface
- The AIShell module for PowerShell

This article explains how to install these packages on your system.

<!-- TODO add details for an installer script for users to run and bypass most of the steps -->

## System requirements

AIShell is supported on the following platforms:

<!-- markdownlint-disable MD023 MD024 MD051 -->
### [Windows](#tab/windows)

- Windows 10 or higher
- PowerShell 7.4 or higher
- Windows Terminal

### [macOS](#tab/macos)

- macOS v13 Ventura or higher
- PowerShell 7.4 or higher
- iTerm2

### [Linux](#tab/linux)

- Ubuntu 20.04 or higher
- PowerShell 7.4 or higher (recommended)
- Any terminal emulator supported by the OS

  > [!NOTE]
  > The AIShell module isn't supported on Linux.

<!-- markdownlint-enable MD023 MD024 MD051 -->

---

## Install AIShell

<!-- markdownlint-disable MD023 MD024 MD051 -->
### [Windows](#tab/windows)

1. Download the latest version from the
   [GitHub releases page][03].
1. Install the AIShell module from the PowerShell Gallery.

   ```powershell
   Install-PSResource -Name AIShell
   ```

### [macOS](#tab/macos)

1. Download the latest version from the
   [GitHub releases page][03].
1. Install the AIShell module from the PowerShell Gallery.

   ```powershell
   Install-PSResource -Name AIShell
   ```

### [Linux](#tab/linux)

1. Download the latest version from the
   [GitHub releases page][03].

<!-- markdownlint-enable MD023 MD024 MD051 -->

---

## Next steps

- [Get started with AIShell][02]
- [Get started with AIShell for PowerShell][01]

<!-- link references -->
[01]: get-started-powershell.md
[02]: get-started-standalone.md
[03]: https://github.com/PowerShell/ProjectMercury/releases/latest
