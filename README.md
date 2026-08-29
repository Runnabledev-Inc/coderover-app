# CodeRover

CodeRover is a free, local-first AI coding agent desktop app for Windows, macOS, and Linux - describe what you need and it edits your code, runs commands, and gets the task done on your own machine.

<p align="center">
  <a href="#install">
    <img alt="Download CodeRover" src="https://img.shields.io/badge/Download-CodeRover-276d70?style=for-the-badge&logo=rocket&logoColor=white">
  </a>
</p>

## About CodeRover

CodeRover is an AI coding agent that runs as a native desktop application on your own machine. Describe what you need in plain language and CodeRover handles the rest - whether you are starting a project from scratch or working in an existing codebase. It reads your code, makes targeted edits, runs builds and tests, searches your project, and works in a loop until the task is done.

Everything runs locally: your code and the commands the agent runs stay on your machine. You review every change in the Changes tab before anything is committed - the agent never commits on its own unless you ask it to.

CodeRover is bring-your-own-key. Connect the AI provider you prefer - Anthropic, OpenAI, any OpenAI-compatible provider, or a local model via Ollama - and you pay that provider directly at cost. There is no subscription and no CodeRover account required.

## Getting started

### Prerequisites

- A modern 64-bit OS: Windows 10/11, macOS 11 (Big Sur) or later, or a Debian/Ubuntu-based Linux distribution.
- An AI provider API key (Anthropic, OpenAI, or any OpenAI-compatible provider). No key? You can point CodeRover at a local model with [Ollama](https://ollama.com) instead.

Everything else - including the Java runtime and database CodeRover uses - is bundled in the installer. No extra setup required.

### Install

Download the latest build for your platform from the [**Releases**](../../releases/latest) page, or use the auto-detecting download button at [coderover.dev](https://coderover.dev):

| Platform | Installer |
| --- | --- |
| Windows 10/11 (x64) | `CodeRover_<version>_x64-setup.exe` |
| macOS (Apple Silicon) | `CodeRover_<version>_aarch64.dmg` |
| macOS (Intel) | `CodeRover_<version>_x64.dmg` |
| Linux (Debian/Ubuntu) | `CodeRover_<version>_amd64.deb` |

On Linux, install the package with `sudo apt install ./CodeRover_<version>_amd64.deb`.

> **Windows:** the installer isn't code-signed yet, so Defender SmartScreen may warn that it's from an "unknown publisher." Click **More info**, then **Run anyway** to continue. You only need to do this once.
>
> **macOS:** builds are not yet notarized by Apple. On first launch, **right-click** (or Control-click) CodeRover in Applications and choose **Open**, then confirm. You only need to do this once.

When you open CodeRover for the first time it starts with a local account - no sign-in required - and takes you straight to the agent. Add your AI provider API key in settings and start chatting. To work on a specific project, attach a folder in the composer before sending your message.

### Updates

CodeRover on **Windows and macOS** updates itself automatically via the built-in updater. On **Linux**, download and reinstall the latest `.deb` to upgrade. You can always grab the newest build from the [Releases](../../releases/latest) page.

## This repository

This repo is the public download and auto-update home for the CodeRover desktop app. Use it to:

- Download releases from the [Releases](../../releases) page
- File bugs and feature requests

Each release includes the per-platform installers, the macOS/Windows updater bundles and their signatures, and a `latest.json` updater manifest.

## Feedback

Report problems or feature requests in the [Issues](../../issues) tab. When filing an issue, please include:

- The app version
- Your operating system and version
- Steps to reproduce
- Expected vs. actual behavior
- Screenshots or videos

## License

© Runnable, Inc. All rights reserved.

## Data & Telemetry

The CodeRover desktop app runs locally and does not send your code or conversations anywhere except to the AI provider you configure. The [coderover.dev](https://coderover.dev) website uses Google Analytics to measure page visits and download clicks so I can improve the product.
