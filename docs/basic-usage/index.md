---
layout: default
title: Basic Usage
nav_order: 3
---

# Basic Usage

Once you have set up Gemini CLI, you can begin interacting with the agent through various interfaces in Sublime Text.

## Opening the Chat Interface

The primary way to interact with Gemini is through the chat view.
1. Use the Command Palette (`Cmd+Shift+P` on macOS, `Ctrl+Shift+P` on Windows/Linux) and search for **`Gemini: Start Chat`**.
2. A new view will open, allowing you to converse with the AI.

### Custom Shortcuts
You can also assign a key binding for faster access:
1. Go to `Preferences -> Package Settings -> GeminiCLI -> Key Bindings`.
2. Add the following to your user settings:
   ```json
   { "keys": ["ctrl+alt+g"], "command": "gemini_cli" }
   ```

## Sending Messages

- **Input**: Type your message in the text input area at the bottom of the chat view.
- **Send**: Press `Ctrl+Enter` (macOS: `Cmd+Enter`) to send the message to Gemini.
- **History**: Use the `Up` and `Down` arrow keys to cycle through your previous prompts.

## Interaction Workflow

1. **Thinking Phase**: Gemini often thinks before responding. You will see an animated indicator while the model processes your query.
2. **Tool Execution**: If Gemini needs to perform an action (e.g., read a file, run a command), it will request your permission.
3. **Diff Review**: When Gemini suggests code changes, it generates a unified diff. You can review the changes and click **Apply** to modify your source files.

## Session Management

To start a fresh conversation, run **`Gemini: Clear Session`** from the command palette. This clears the context and allows you to focus on a new task without interference from previous messages.
