# Automation Suite Guide

The Automation Suite is a centralised dashboard for accessing the Platform Integrity (PI) and Usage Control (UC) automation modules.

---

## Overview

The Automation Suite allows you to launch module-specific automation tools and download required templates for your configuration work.

📷 [INSERT SCREENSHOT: automation_suite.png]

---

## Understanding the Interface

### Module Cards

The dashboard displays three module cards:

| Module | Status | Description |
|--------|--------|-------------|
| **Usage Control (UC)** | Available | Data pipeline and validation automation for UC |
| **Platform Integrity (PI)** | Available | Validation rules and dashboard configuration for PI |
| **Fraud Management (FMS)** | Coming Soon | Data pipeline automation for FMS (not yet available) |

### Each Card Contains

- **Module Name** — Identifies the module
- **Description** — Brief explanation of the module's purpose
- **Launch Button** — Opens the module's automation dashboard
- **Download Templates Button** — Downloads the required input templates

---

## How to Launch a Module

### Step 1: Select Your Module
Identify the module you need to work with (UC or PI).

### Step 2: Click Launch
Click the **Launch** button on the respective card.

### Step 3: Module Dashboard Opens
The selected module's dashboard will open in the same window, showing all available operations.

---

## How to Download Templates

Before running automation, you may need input template files. Here is how to download them:

### Step 1: Click Download Templates
On the module card, click the **Download Templates** button.

### Step 2: Templates Are Saved
The templates are automatically saved to your Downloads folder:
- Location: `Downloads/Automation_Suite_Templates/{Module}_Templates/`

### Step 3: Open Folder (Optional)
A prompt will ask if you want to open the folder. Click **Yes** to view the downloaded files.

📷 [INSERT SCREENSHOT: automation_suite_download_success.png]

---

## Available Modules

### Usage Control (UC)

The UC module provides 19 automation operations:

| Category | Operations |
|----------|------------|
| **Entity Creation** | Aggregate and detailed entity creation |
| **Data Pipeline** | Formats, streams, schema mappings, bindings |
| **Validations** | Aggregate, detailed, and inter-system validations |
| **Dashboards** | Trend, file sequence, alarm, and mismatch dashboards |

For detailed instructions, see the [UC Module Guide](uc_module/01_Overview.md).

---

### Platform Integrity (PI)

The PI module provides 13 automation operations:

| Category | Operations |
|----------|------------|
| **Entity Creation** | Entity, dump, and view table creation |
| **Data Pipeline** | Formats, streams, bindings |
| **Validations** | Inter-system and intra-system validations |
| **Dashboards** | Inter-system and intra-system dashboards |

For detailed instructions, see the [PI Module Guide](pi_module/01_Overview.md).

---

## Using the Help Feature

The Automation Suite includes a built-in help feature that provides detailed information about each module.

### Accessing Help
Click the **Help** button in the header section.

📷 [INSERT SCREENSHOT: automation_suite_help.png]

### Help Content Includes
- Available operations for each module
- Required input file formats
- Step-by-step workflow guidance

---

## Tips for Using the Automation Suite

| Tip | Description |
|-----|-------------|
| **Download templates first** | Ensure you have the correct input files before running operations |
| **Complete operations in order** | Some operations depend on outputs from previous steps |
| **Check operation status** | Monitor the status of running operations in the dashboard |

---

## Next Steps

Choose the module you want to work with:

- [UC Module Guide](uc_module/01_Overview.md) — Detailed guide for Usage Control operations
- [PI Module Guide](pi_module/01_Overview.md) — Detailed guide for Platform Integrity operations
- [SDD Automation Tool Guide](sdd_automation_tool/01_Overview.md) — Guide for SDD management

---

**← [Back to Home](00_Home.md)**
