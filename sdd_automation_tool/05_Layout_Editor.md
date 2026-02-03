# Layout Editor

This guide explains how to create and edit layouts in the SDD Automation Tool. Layouts define the structure and format of your source data.

---

## What is a Layout?

A layout defines the structure of your source data, including:

- Field names and order
- Data format (ASN1, XML, JSON, or DSV)
- Field structure and hierarchy

---

## Opening the Layout Editor

### For New Layouts

1. Create a metadata entry first (if not already created)
2. Click **Edit** on the entry row and select **Edit Layout**
3. A new layout editor window opens

### For Existing Layouts

1. Locate the entry with the layout
2. Click **Edit** on the entry row and select **Edit Layout**
3. The existing layout opens for editing

📷 [INSERT SCREENSHOT: sdd_layout_editor_full.png]

---

## Understanding the Layout Editor Interface

### Header Section

| Element | Description |
|---------|-------------|
| **Entry Information** | Shows the source, vendor, and source name |
| **Format Selection** | Choose the data format type |

### Format Selection

Select the format that matches your source data:

📷 [INSERT SCREENSHOT: sdd_layout_format_select.png]

| Format | When to Use |
|--------|-------------|
| **ASN1** | When source data is in ASN.1 format |
| **XML** | When source data is in XML format |
| **JSON** | When source data is in JSON format |
| **DSV** | When source data is delimited (CSV, pipe-separated, etc.) |

---

## Creating a Layout in Text Mode (ASN1, XML, JSON)

For ASN1, XML, and JSON formats, you enter the layout definition as text.

### Step 1: Select the Format

Choose ASN1, XML, or JSON from the format dropdown.

### Step 2: Enter the Layout Definition

Enter your layout definition in the text area provided.

### Step 3: Save the Layout

Click **Save** to save the layout.

---

## Creating a Layout in DSV Mode

For DSV (Delimited Separated Values) format, you upload an Excel file containing the field definitions.

### Step 1: Select DSV Format

Choose DSV from the format dropdown.

### Step 2: Upload the Layout File

Click **Upload File** and select your Excel file.

### Step 3: Review the Preview

After uploading, a preview of the fields appears.

### Step 4: Save the Layout

Click **Save** to save the layout.

---

## DSV File Requirements

When using DSV format, your Excel file must meet these requirements:

| Requirement | Description |
|-------------|-------------|
| **Field Name column** | Must contain a column named "Field Name" |
| **One field per row** | Each row represents one field |
| **No empty rows** | Remove any empty rows before uploading |

---

## Editing an Existing Layout

### Step 1: Open the Layout

Click **Edit** on the entry row and select **Edit Layout**.

### Step 2: Make Changes

- For text formats: Edit the text directly
- For DSV format: Upload a new file or edit the table

### Step 3: Save Changes

Click **Save** to save your changes.

---

## Layout Naming Convention

Layout files are named using the following pattern:

**{LoadingFlow}_Layout.xlsx** (for DSV)

or

**{LoadingFlow}_Layout.txt** (for text formats)

Example: `ld_CDR_Layout.xlsx`

---

## Tips for Working with Layouts

| Tip | Description |
|-----|-------------|
| **Match the source format** | Select the format that matches your actual source data |
| **Preserve field order** | Keep fields in the same order as the source |
| **Use consistent naming** | Use consistent field naming conventions |
| **Validate before saving** | Review the layout before saving |

---

## Next Steps

- [Version Control](06_Version_Control.md) — Learn how to manage versions
- [Loading Rule Editor](04_Loading_Rule_Editor.md) — Learn about loading rule configuration

---

**← [Back to SDD Overview](01_Overview.md)**
