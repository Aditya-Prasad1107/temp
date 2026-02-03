# NOVA Launcher Guide

The NOVA Launcher is your starting point for all automation activities. This guide explains how to use the launcher to access your automation tools.

---

## Overview

The NOVA Launcher provides a simple, modern interface for launching automation tools. It manages multiple tools simultaneously and keeps track of running processes.

📷 [INSERT SCREENSHOT: nova_launcher_main.png]

---

## Understanding the Interface

When you open the NOVA Launcher, you will see the following sections:

### Header Section
- Displays the **NOVA** branding and version number
- Shows the acronym expansion: "Next-generation Orchestration via Versatile Automation"

### Automation Cards
Each card represents an available tool:
- **Automation Suite (Standalone)** — For PI and UC automation
- **SDD Automation Tool** — For SDD management and RAID configuration

### Footer Section
- Shows the current status
- Provides an **Exit** button to close the launcher

---

## How to Launch an Automation Tool

### Step 1: Click the Launch Button
Locate the automation card you want to use and click the **Launch Automation** button.

### Step 2: Wait for Loading
A loading indicator will appear while the tool starts. This typically takes a few seconds.

### Step 3: Tool Opens
The selected tool will open in a new window. The NOVA Launcher remains open so you can launch additional tools if needed.

---

## Managing Running Tools

### Viewing Active Processes
The footer displays how many automation tools are currently running.

### Exiting with Running Tools
If you try to exit while tools are still running, you will see a confirmation message.

📷 [INSERT SCREENSHOT: nova_launcher_exit_confirmation.png]

**Options:**
- Click **Yes** to close all running tools and exit
- Click **No** to cancel and keep everything running

---

## Available Automation Tools

### Automation Suite (Standalone)

| Feature | Description |
|---------|-------------|
| **Purpose** | Access Platform Integrity and Usage Control automation modules |
| **When to Use** | When you need to create entities, validations, or dashboards |

### SDD Automation Tool

| Feature | Description |
|---------|-------------|
| **Purpose** | Manage System Design Documents with version control |
| **When to Use** | When you need to create or edit loading rules, layouts, or configure RAID |

---

## Tips for Best Results

| Tip | Explanation |
|-----|-------------|
| **Keep the launcher open** | You can launch multiple tools without closing the launcher |
| **Check the console** | Progress messages appear in the console window |
| **Exit properly** | Always use the Exit button to ensure all processes close correctly |

---

## Troubleshooting

### Tool Does Not Launch
- Wait a few seconds — some tools take time to initialise
- Check if Chrome is installed (required for RAID features)
- Try launching again if the first attempt fails

### Launcher Closes Unexpectedly
- Reopen the NOVA Launcher
- Check the console for any error messages
- Contact support if the problem persists

---

## Next Steps

Now that you understand the NOVA Launcher, choose your next guide:

- [Automation Suite Guide](02_Automation_Suite.md) — Learn how to use PI and UC modules
- [SDD Automation Tool Guide](sdd_automation_tool/01_Overview.md) — Learn how to manage SDD documents

---

**← [Back to Home](00_Home.md)**
