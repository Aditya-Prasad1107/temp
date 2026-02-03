# UC Module Guide

The Usage Control (UC) Module provides automation for UC-related configurations in the RAID system.

---

## Overview

The UC Module helps you automate:

- Aggregate and detailed entity creation
- Data pipeline configuration
- Control point validations
- Trending, file sequence, and mismatch validations
- Dashboard creation

📷 [INSERT SCREENSHOT: uc_dashboard.png]

---

## Accessing the UC Module

### Step 1: Open the Automation Suite

From the NOVA Launcher, launch the **Automation Suite (Standalone)**.

### Step 2: Launch UC

Click the **Launch** button on the UC card.

### Step 3: UC Dashboard Opens

The UC Dashboard displays all available operations.

---

## Available Operations

The UC Module provides 19 automation operations organised into categories:

### Entity Creation

| Operation | Description |
|-----------|-------------|
| **Aggregate Entity Creation** | Create aggregate entities |
| **Detailed Entity Creation** | Create detailed entities |

### Data Pipeline

| Operation | Description |
|-----------|-------------|
| **Formats Creation** | Define data formats |
| **Streams Creation** | Configure data streams |
| **Schema Mappings** | Configure schema mappings |
| **Bindings Creation** | Create bindings between components |

### Control Points

| Operation | Description |
|-----------|-------------|
| **Control Point Creation** | Create control points |
| **Control Point Validation** | Validate control points |

### Validations

| Operation | Description |
|-----------|-------------|
| **Aggregate Validation** | Validate aggregate data |
| **Detailed Validation** | Validate detailed data |
| **Inter-System Validation** | Configure inter-system validations |
| **Trending Validation** | Set up trending validations |
| **File Sequence Validation** | Configure file sequence checks |
| **Mismatch Validation** | Configure mismatch detection |

### Dashboards

| Operation | Description |
|-----------|-------------|
| **Trend Dashboard** | Create trending dashboards |
| **File Sequence Dashboard** | Create file sequence dashboards |
| **Alarm Dashboard** | Create alarm dashboards |
| **Mismatch Dashboard** | Create mismatch dashboards |

### Other

| Operation | Description |
|-----------|-------------|
| **Full Automation** | Run complete automation workflow |

---

## Running an Operation

### Step 1: Select the Operation

Click on the operation you want to run.

### Step 2: Provide Input Files (If Required)

Some operations require input files. A file selection dialog will appear.

### Step 3: Operation Runs

The operation begins processing. Progress is displayed.

📷 [INSERT SCREENSHOT: uc_operation_running.png]

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
| **Control Point Template** | Define control points |

### File Format

All input files should be in Excel format (.xlsx).

---

## Common Workflow

A typical UC workflow follows these steps:

| Step | Operation | Description |
|------|-----------|-------------|
| 1 | Aggregate Entity Creation | Create aggregate entities first |
| 2 | Detailed Entity Creation | Create detailed entities |
| 3 | Formats Creation | Define data formats |
| 4 | Streams Creation | Configure data streams |
| 5 | Schema Mappings | Set up schema mappings |
| 6 | Bindings Creation | Bind components together |
| 7 | Control Point Creation | Create control points |
| 8 | Validations | Set up required validations |
| 9 | Dashboards | Create monitoring dashboards |

---

## Tips for Using the UC Module

| Tip | Description |
|-----|-------------|
| **Follow the order** | Complete operations in the recommended order |
| **Use templates** | Always start with the provided templates |
| **Check outputs** | Verify each operation's output before proceeding |
| **Complete prerequisites** | Ensure earlier operations are done before later ones |

---

## Next Steps

- [PI Module Guide](../pi_module/01_Overview.md) — Learn about PI automation
- [SDD Automation Tool](../sdd_automation_tool/01_Overview.md) — Learn about SDD management

---

**← [Back to Automation Suite](../02_Automation_Suite.md)** | **← [Back to Home](../00_Home.md)**
