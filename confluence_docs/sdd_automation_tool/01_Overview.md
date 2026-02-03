# SDD Automation Tool - Overview

The SDD Automation Tool is a comprehensive application for managing System Design Documents (SDD), loading rules, layouts, and RAID integration.

---

## What is the SDD Automation Tool?

The SDD Automation Tool helps you:

- Manage metadata for your data sources
- Create and edit loading rules
- Define data layouts in various formats
- Track versions of your configurations
- Generate consolidated SDD reports
- Configure RAID automation settings

📷 [INSERT SCREENSHOT: sdd_main_window.png]

---

## Key Features

| Feature | Description |
|---------|-------------|
| **Destination Management** | Select folders for storing your SDD data |
| **Metadata Tracking** | Maintain records of all loading rules and layouts |
| **Loading Rule Editor** | Create and edit loading rules from templates |
| **Layout Editor** | Define data layouts in ASN1, XML, JSON, or DSV formats |
| **Version Control** | Track changes with automatic versioning |
| **SDD Consolidation** | Generate comprehensive Excel reports |
| **RAID Integration** | Configure and automate RAID portal settings |

---

## Main Window Overview

When you open the SDD Automation Tool, you will see the main window divided into several sections:

### Top Bar

| Button | Purpose |
|--------|---------|
| **Select Destination Folder** | Choose where to store your SDD data |
| **DataType Mappings** | Configure field-to-datatype mappings |
| **Columns** | Show or hide table columns |
| **Refresh** | Reload the metadata table |

### Metadata Table

The central area displays all your metadata entries in a table format. Each row represents one configuration entry.

### Bottom Bar

| Button | Purpose |
|--------|---------|
| **Create New Entry** | Add a new metadata entry |
| **RAID Config Params** | Configure RAID automation settings |
| **Consolidate SDD** | Generate a consolidated Excel report |
| **Close** | Exit the application |

---

## Getting Started

### Step 1: Launch the SDD Automation Tool

From the NOVA Launcher, click **Launch Automation** on the SDD Automation Tool card.

### Step 2: Select a Destination Folder

When the tool opens, you will be prompted to select a destination folder. This is where all your SDD data will be stored.

📷 [INSERT SCREENSHOT: sdd_destination_dialog.png]

**Note:** The tool remembers your last selected folder, so you will not need to select it again on subsequent launches.

### Step 3: View Your Entries

If the folder contains existing data, your entries will appear in the metadata table. If this is a new folder, the table will be empty.

---

## Table Columns Explained

The metadata table displays the following information for each entry:

| Column | Description |
|--------|-------------|
| **Applicable Domain** | RA or FMS |
| **Module** | UC or PI |
| **Source** | Data source identifier |
| **Vendor** | Vendor name |
| **Vendor Version** | Vendor version number |
| **Source Name** | Descriptive name for the source |
| **Loading Rule** | Name of the loading rule file |
| **Layout** | Name of the layout file |
| **Current Version** | Current version number |
| **Last Finalized Version** | Last finalized version |
| **Actions** | Action buttons for the entry |

---

## Action Buttons

Each entry row has action buttons:

📷 [INSERT SCREENSHOT: sdd_action_buttons.png]

| Button | Purpose |
|--------|---------|
| **Edit** | Opens a menu to edit metadata, loading rule, or layout |
| **View** | View the loading rule or layout (read-only) |
| **Delete** | Remove the loading rule, layout, or metadata entry |
| **Finalize** | Mark the current version as finalized and create a new version |
| **⋮ (More)** | Additional options (open in explorer, copy path, export) |

---

## In This Section

| Page | What You Will Learn |
|------|---------------------|
| [Creating Entries](02_Creating_Entries.md) | How to create new metadata entries |
| [Editing Entries](03_Editing_Entries.md) | How to edit existing entries |
| [Loading Rule Editor](04_Loading_Rule_Editor.md) | How to create and edit loading rules |
| [Layout Editor](05_Layout_Editor.md) | How to create and edit layouts |
| [Version Control](06_Version_Control.md) | How to manage versions |
| [DataType Mappings](07_DataType_Mappings.md) | How to configure datatype mappings |
| [RAID Configuration](08_RAID_Configuration.md) | How to configure RAID settings |
| [SDD Consolidation](09_SDD_Consolidation.md) | How to generate consolidated reports |

---

**← [Back to Home](../00_Home.md)**
