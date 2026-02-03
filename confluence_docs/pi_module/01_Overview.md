# PI Module Guide

The Platform Integrity (PI) Module provides automation for PI-related configurations in the RAID system.

---

## Overview

The PI Module helps you automate:

- Entity creation and management
- Format and stream configuration
- Inter-system and intra-system validations
- Dashboard creation

📷 [INSERT SCREENSHOT: pi_dashboard.png]

---

## Accessing the PI Module

### Step 1: Open the Automation Suite

From the NOVA Launcher, launch the **Automation Suite (Standalone)**.

### Step 2: Launch PI

Click the **Launch** button on the PI card.

### Step 3: PI Dashboard Opens

The PI Dashboard displays all available operations.

---

## Available Operations

The PI Module provides 13 automation operations organised into categories:

### Entity Creation

| Operation | Description |
|-----------|-------------|
| **Entity Creation** | Create entities in the RAID system |
| **Dump Table Creation** | Create dump tables for data loading |
| **View Table Creation** | Create views for data access |

### Data Pipeline

| Operation | Description |
|-----------|-------------|
| **Formats Creation** | Define data formats |
| **Streams Creation** | Configure data streams |
| **Bindings Creation** | Create bindings between formats and streams |

### Validations

| Operation | Description |
|-----------|-------------|
| **Inter-System Validation** | Configure validations between systems |
| **Intra-System Validation** | Configure validations within a system |

### Dashboards

| Operation | Description |
|-----------|-------------|
| **Inter-System Dashboard** | Create inter-system dashboards |
| **Intra-System Dashboard** | Create intra-system dashboards |

### Other

| Operation | Description |
|-----------|-------------|
| **Clone Configuration** | Clone existing configurations |
| **Full Automation** | Run complete automation workflow |
| **Schema Mappings** | Configure schema mappings |

---

## Running an Operation

### Step 1: Select the Operation

Click on the operation you want to run.

### Step 2: Provide Input Files (If Required)

Some operations require input files. A file selection dialog will appear.

### Step 3: Operation Runs

The operation begins processing. Progress is displayed.

📷 [INSERT SCREENSHOT: pi_operation_running.png]

### Step 4: Monitor Progress

Monitor the status in the operation panel.

### Step 5: Completion

When complete, a status message appears indicating success or any issues.

---

## Aborting an Operation

If you need to stop a running operation:

1. Click the **Abort** button
2. Confirm the abortion
3. The operation stops

---

## Input File Requirements

### Template Files

Download templates from the Automation Suite before running operations.

| Template | Purpose |
|----------|---------|
| **Entity Template** | Define entity configuration |
| **Format Template** | Define format specifications |
| **Stream Template** | Define stream configuration |
| **Validation Template** | Define validation rules |

### File Format

All input files should be in Excel format (.xlsx).

---

## Common Workflow

A typical PI workflow follows these steps:

| Step | Operation | Description |
|------|-----------|-------------|
| 1 | Entity Creation | Create entities first |
| 2 | Formats Creation | Define data formats |
| 3 | Streams Creation | Configure data streams |
| 4 | Bindings Creation | Bind formats to streams |
| 5 | Inter-System Validation | Set up validations |
| 6 | Inter-System Dashboard | Create dashboards |

---

## Tips for Using the PI Module

| Tip | Description |
|-----|-------------|
| **Follow the order** | Complete operations in the recommended order |
| **Use templates** | Always start with the provided templates |
| **Check outputs** | Verify each operation's output before proceeding |
| **Save logs** | Keep operation logs for troubleshooting |

---

## Next Steps

- [UC Module Guide](../uc_module/01_Overview.md) — Learn about UC automation
- [SDD Automation Tool](../sdd_automation_tool/01_Overview.md) — Learn about SDD management

---

**← [Back to Automation Suite](../02_Automation_Suite.md)** | **← [Back to Home](../00_Home.md)**
