# Loading Rule Editor

This guide explains how to create and edit loading rules in the SDD Automation Tool. Loading rules define how data fields are mapped and processed.

---

## What is a Loading Rule?

A loading rule is a configuration that defines:

- The fields to be processed
- How each field is mapped from the source layout
- Lookup table associations
- Additional comments or notes

---

## Opening the Loading Rule Editor

### For New Loading Rules

1. Create a metadata entry first (if not already created)
2. Click **Edit LR** on the entry row
3. You will be prompted to select a source folder

### For Existing Loading Rules

1. Locate the entry with the loading rule
2. Click **Edit LR** on the entry row
3. The existing loading rule opens for editing

📷 [INSERT SCREENSHOT: sdd_loading_rule_editor_full.png]

---

## Understanding the Loading Rule Editor Interface

### Header Section

| Element | Description |
|---------|-------------|
| **Entry Information** | Shows the source, vendor, and module |
| **Version Information** | Shows the current version number |

### Table Section

The main area displays the loading rule data in a table format:

| Column | Description |
|--------|-------------|
| **ID** | Unique identifier for each field |
| **Dim./ Meas.** (UC) or **Keys / Att.** (PI) | Field type indicator |
| **Name** | Field name |
| **Mapping (from layout)** | How the field is mapped from the source layout |
| **Lookup Table** | Associated lookup table (if any) |
| **Comments** | Additional notes about the field |

### For PI Module Only

If working with a PI module entry, you may see additional columns:

| Column | Description |
|--------|-------------|
| **SUBS** | Subscriber configuration |
| **SERV** | Service configuration |
| **PACK** | Package configuration |
| **DEV** | Device configuration |

---

## Creating a New Loading Rule

### Step 1: Select Source Folder

When prompted, navigate to and select the source folder containing your template files.

### Step 2: Template is Loaded

The editor loads the template and displays the fields.

### Step 3: Configure Field Mappings

For each field, configure the mapping:

1. Click on the **Mapping (from layout)** cell
2. A dropdown appears with available options
3. Select the appropriate mapping

📷 [INSERT SCREENSHOT: sdd_loading_rule_dropdown.png]

### Step 4: Add Lookup Tables (If Needed)

Fill in the **Lookup Table** column where required.

### Step 5: Add Comments (Optional)

Add any notes or comments to the **Comments** column.

---

## Adding and Removing Rows

### Adding a New Row

1. Click the **Add Row** button
2. A new empty row appears at the bottom
3. Fill in the required fields

### Removing a Row

1. Select the row you want to delete
2. Click the **Delete Row** button
3. Confirm the deletion

---

## Saving the Loading Rule

When you are ready to save your changes:

1. Click the **Save** button
2. Changes are saved to the current version file

> [!NOTE]
> The Save action overwrites the current version. It does not create a new version. To create a new version, use the **Finalize** button from the main metadata table (see [Version Control](06_Version_Control.md)).

---


## Version Naming Convention

Loading rule files are named using the following pattern:

**{Source}_{Vendor}_{VendorVersion}_LdRules_{FileName}_v{Version}**

Example: `SAP_Vendor1_2.0_LdRules_CDR_v3`

---

## Finalising a Version

When you are satisfied with a version and it is ready for use:

1. Return to the main window
2. Find your entry in the table
3. Select the version in the **Current Version** dropdown
4. Click **Finalize** button

📷 [INSERT SCREENSHOT: sdd_finalize_button.png]

The **Last Finalized Version** column will update to show the finalized version.

For more details on version management, see [Version Control](06_Version_Control.md).

---

## Tips for Working with Loading Rules

| Tip | Description |
|-----|-------------|
| **Review before saving** | Check all mappings before saving |
| **Use comments** | Document any non-obvious mappings |
| **Create versions** | Create new versions for significant changes |
| **Finalize when ready** | Finalize versions that are ready for production |

---

## Next Steps

- [Layout Editor](05_Layout_Editor.md) — Learn how to create and edit layouts
- [Version Control](06_Version_Control.md) — Learn how to manage versions

---

**← [Back to SDD Overview](01_Overview.md)**
