# BrickWire — AI-Powered Roblox Studio Automation

**BrickWire** is a free, open-source browser extension that connects AI chat platforms directly to Roblox Studio, turning supported AI models into hands-on development agents.

Control Roblox Studio through a normal AI conversation. Read and edit scripts, execute Luau, inspect instances, generate assets, browse the Creator Store, and automate playtesting — without API keys, terminal commands, or manually writing every line of code.

A free alternative to Lemonade.gg and Luamotion for building Roblox games with AI.

## Supported AI Providers

BrickWire supports eight browser-based AI platforms:

- **DeepSeek** — Recommended provider.
- **ChatGPT** — Image input and screenshots are disabled by design.
- **Google Gemini** — May stop invoking Roblox tools during longer sessions.
- **Kimi** — May prioritize native tools over BrickWire commands.
- **GLM** — Powered by Z.ai.
- **Qwen** — Browser-based AI platform.
- **Arena** — Direct mode only; Battle, Side-by-Side, and Agent modes are unsupported.
- **Meta AI** — Supported browser-based provider.

> 💬 **Community & Support:** [Join the Discord](https://discord.gg/9aNyZsMWcb)

## Architecture

BrickWire connects browser-based AI conversations to Roblox Studio through a local bridge and Studio's built-in MCP server.

```text
AI Chat Platform
       │
       ▼
BrickWire Browser Extension
       │
       ▼
Local Bridge
       │
       ▼
Roblox Studio MCP Server
       │
       ▼
Roblox Game Project
```

The extension operates within supported AI chat websites. Requests are translated into commands handled by the local Bridge, enabling the selected AI model to interact with Roblox Studio through the available tools.

## Installation

### 1. Download BrickWire

Download the latest release archive from the official project's Releases page and extract it.

Install the browser extension:

1. Open `chrome://extensions` in Chrome or `edge://extensions` in Microsoft Edge.
2. Enable **Developer mode**.
3. Select **Load unpacked**.
4. Choose the `zeroscript-extension` folder from the extracted archive.

### 2. Enable Roblox Studio MCP

Open Roblox Studio and load your place.

Navigate to:

**Assistant AI → `...` → Manage MCP Servers → Enable Studio as MCP Server**

### 3. Start the BrickWire Bridge

Launch the appropriate file from the extracted archive:

- **Windows:** `start.bat`
- **macOS:** `MacOS_Start.command`

Keep the Bridge running while using BrickWire.

On macOS, downloaded launchers may trigger a security warning. Verify the file's source before allowing it to run, then review the available options under **System Settings → Privacy & Security**.

### 4. Start an AI Session

Open one of the supported AI platforms:

| Provider | Website |
|---|---|
| DeepSeek | https://chat.deepseek.com |
| ChatGPT | https://chatgpt.com |
| Google Gemini | https://gemini.google.com |
| Kimi | https://www.kimi.ai |
| GLM | https://chat.z.ai |
| Qwen | https://chat.qwen.ai |
| Arena | https://arena.ai |
| Meta AI | https://www.meta.ai |

Start a new conversation and locate the BrickWire interface above the message input.

Select **Start session**, then describe what you want to build or modify in Roblox Studio.

**Recommended configuration:** DeepSeek with a fresh conversation. Arena requires Direct mode.

### Setup Tutorial

Watch the setup walkthrough: https://youtu.be/kPKiZLZ9_Ps

## Features

BrickWire enables AI-assisted Roblox development through natural-language instructions.

- **Script Editing** — Read, create, and modify Luau scripts.
- **Luau Execution** — Execute code directly in Roblox Studio.
- **Game Inspection** — Inspect the Explorer hierarchy, instances, and project structure.
- **Asset Generation** — Generate meshes, materials, and models.
- **Creator Store Integration** — Browse and insert assets.
- **Playtest Automation** — Control supported testing workflows.
- **Persistent Project Memory** — Store project context inside the place for future sessions.

Capabilities and reliability depend on the selected AI model, available tools, and current session.

## Compatibility & Limitations

- Works only on the eight supported AI chat domains.
- DeepSeek is the recommended provider.
- ChatGPT image input and screenshots are disabled by design.
- Gemini may stop using Roblox tools in longer sessions.
- Kimi may use its own native tools instead of BrickWire commands.
- Arena supports Direct mode only.
- If the model stops executing commands, remind it to use BrickWire's Roblox tools or start a fresh session.

## Free & Open Source

BrickWire is intended to remain free and open-source. There is no official paid edition or mandatory sign-in.

Be cautious of third-party websites or extensions using the BrickWire name that request payment or account credentials.

Use the official project links for releases, documentation, and updates.

---

**BrickWire — Your AI. Your Studio. Your Game.**
