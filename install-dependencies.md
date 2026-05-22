[&larr; Back to Workshop Home](index.html)

# Open the Terminal, Install Dependencies, and Start an Agent

This page matches the hands-on setup in the slides. Work through it in order and run the commands one at a time.

---

## Step 1: Open the Terminal

### macOS

1. Press `Cmd + Space` to open Spotlight.
2. Type **Terminal**.
3. Press `Return`.

You can also open **Applications -> Utilities -> Terminal**.

### Windows

1. Open **Command Prompt** or **PowerShell**.
2. If WSL is not already installed, run:

```bash
wsl --install Ubuntu
```

3. Start WSL:

```bash
wsl
```

The first-time setup may ask for a username and password.

4. Once you are inside WSL, install the Linux packages the workshop apps may need:

```bash
sudo apt install libgconf-2-4 libatk1.0-0 libatk-bridge2.0-0 libgdk-pixbuf2.0-0 libgtk-3-0 libgbm-dev libnss3-dev libxss-dev
```

---

## Step 2: Install Dependencies

### 1. Install Homebrew

Homebrew is a package manager. It helps install the software we need with simple terminal commands.

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

When the install finishes, Homebrew may ask you to copy, paste, and run a few extra commands. Run each one separately in the terminal.

### 2. Install Node.js

Node.js is the runtime used by the coding agents we are installing.

```bash
brew install nodejs
```

---

## Step 3: Install an Agent

Choose one agent and install it. You only need to do this once.

**Important:** install the agent only. Do not start it yet. We will do that together in Step 5.

### Claude Code

```bash
npm install -g @anthropic-ai/claude-code
```

### Codex

```bash
npm install -g @openai/codex
```

### Gemini

```bash
npm install -g @google/gemini-cli
```

---

## Step 4: Make a Workshop Folder

Create a clean place for today's project:

```bash
mkdir workshop
```

Step into it:

```bash
cd workshop
```

---

## Step 5: Start an Agent

Start the agent from inside your `workshop` folder.

### Claude Code

```bash
claude
```

### Codex

```bash
codex
```

### Gemini

```bash
gemini
```

---

## Step 6: Choose a Model and Thinking Level

### Claude Code

Use this inside Claude Code:

```text
/model
```

Pick **Opus** for more complicated tasks and **Sonnet** for simpler everyday tasks.

Then set effort to auto:

```text
/effort auto
```

### Codex

Use this inside Codex:

```text
/model
```

Use the strongest/default coding model for harder tasks, or the smaller/mini model for simpler tasks. Set reasoning to **medium** for now and turn it up later only if the task is genuinely hard.

---

**Next step:** [Setup Prompt &rarr;](setup-prompt.html)
