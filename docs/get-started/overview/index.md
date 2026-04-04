# Overview

Gemini CLI for Sublime Text provides an agentic interface to the Google Gemini AI directly within your editor. Unlike traditional chatbots, this integration allows Gemini to act as a co-developer that can read files, execute commands, and search the web to help you build software more efficiently.

By leveraging the `@google/gemini-cli` tool, this plugin brings advanced AI capabilities—like context-aware code generation and automated task execution—into the familiar Sublime Text environment.

## Key Features

- **Agentic Interface**: Gemini can actively interact with your workspace by reading files, listing directories, and even executing shell commands (with your permission).
- **Direct Sublime Integration**: Interact via a specialized chat view, command palette, and context menus.
- **Context-Aware**: Easily provide specific files or code selections to Gemini using `@filename` mentions.
- **Privacy First**: Data is only sent when you explicitly mention files or when the agent requests permission to read something.
- **Seamless Diff Workflow**: Review proposed code changes in a unified diff format and apply them with a single click.

## How it Works

The plugin acts as a client that spawns and communicates with the `gemini` command-line tool over standard I/O streams using JSON. This ensures that the heavy lifting is handled by the CLI, while Sublime Text remains responsive and provides a rich UI for interaction.
