# SDD Consolidation

This guide explains how to generate consolidated SDD reports in the SDD Automation Tool.

---

## What is SDD Consolidation?

SDD Consolidation combines all your metadata entries into a single, comprehensive Excel report. This report includes:

- All loading rules
- All layouts
- Metadata information
- Version details

---

## Prerequisites for Consolidation

Before you can consolidate, ensure the following:

| Requirement | Description |
|-------------|-------------|
| **At least one entry** | You need entries to consolidate |
| **Finalized versions** | Entries should have finalized versions |
| **Complete metadata** | All required fields should be filled |

---

## Opening the Consolidation Feature

### Step 1: Check the Button State

The **Consolidate SDD** button at the bottom of the main window is enabled when entries exist.

### Step 2: Click Consolidate SDD

Click the **Consolidate SDD** button.

---

## Consolidation Process

### Step 1: Validation

The tool first validates all entries:

| Validation | What is Checked |
|------------|-----------------|
| **Required fields** | All required metadata fields are filled |
| **Loading Flow format** | Loading Flow starts with "ld_" |
| **Sheet name length** | Generated sheet names are within Excel limits |
| **Finalized versions** | Entries have finalized loading rules |
| **File existence** | Loading rule and layout files exist |

### Step 2: Validation Results

If validation fails, you will see a report of issues:

📷 [INSERT SCREENSHOT: sdd_consolidation_validation_error.png]

The report shows:

| Information | Description |
|-------------|-------------|
| **Entry details** | Which entry has the issue |
| **Issue description** | What needs to be corrected |
| **Recommended action** | How to fix the issue |

### Step 3: Fix Issues (If Any)

If issues are found:

1. Close the consolidation dialog
2. Fix the issues in the affected entries
3. Try consolidation again

---

## Successful Consolidation

If all entries pass validation:

### Step 1: Consolidation Begins

A progress dialog appears showing the consolidation status.

### Step 2: Progress Updates

The dialog shows which entries are being processed.

### Step 3: Completion

When finished, a success message appears.

📷 [INSERT SCREENSHOT: sdd_consolidation_success.png]

### Step 4: Output File Location

The consolidated file is saved in your destination folder.

---

## Understanding the Consolidated Report

The consolidated Excel file contains multiple sheets:

### Summary Sheet

Contains an overview of all entries with key metadata.

### Loading Rule Sheets

One sheet per entry containing the loading rule data.

Sheet naming convention: `LdRules_{LoadingFlow}`

### Layout Sheets

One sheet per entry containing the layout data.

Sheet naming convention: `Layout_{LoadingFlow}`

---

## Common Validation Errors

### Missing Required Fields

| Error | Solution |
|-------|----------|
| "Source Name is empty" | Edit the entry and add the source name |
| "Loading Flow is empty" | Edit the entry and add the loading flow |
| "Phase is not set" | Edit the entry and set the phase |
| "Request ID is not set" | Edit the entry and add the request ID |

### Format Errors

| Error | Solution |
|-------|----------|
| "Loading Flow must start with 'ld_'" | Edit the loading flow to start with "ld_" |
| "Sheet name too long" | Use a shorter loading flow name |

### Missing Files

| Error | Solution |
|-------|----------|
| "No loading rule file exists" | Create a loading rule for the entry |
| "No layout file exists" | Create a layout for the entry |
| "No finalized version exists" | Finalize a version of the loading rule |

---

## Best Practices for Consolidation

| Practice | Description |
|----------|-------------|
| **Finalize before consolidating** | Ensure all entries have finalized versions |
| **Review validation results** | Address all issues before proceeding |
| **Keep backups** | Keep copies of important consolidated reports |
| **Verify output** | Open the consolidated file and verify content |

---

## Next Steps

After consolidation, you may want to:

- Review the consolidated report
- Share the report with stakeholders
- Use the report for RAID configuration
- Archive the report for record-keeping

---

**← [Back to SDD Overview](01_Overview.md)**
