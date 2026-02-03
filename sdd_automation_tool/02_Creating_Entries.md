# Creating Entries

This guide explains how to create new metadata entries in the SDD Automation Tool.

---

## What is a Metadata Entry?

A metadata entry is a record that stores all information about a specific data source configuration. Each entry includes:

- Source and vendor details
- Loading rule and layout references
- Version tracking information
- RAID configuration links

---

## How to Create a New Entry

### Step 1: Click Create New Entry

In the main window, click the **Create New Entry** button at the bottom of the screen.

### Step 2: The Metadata Dialog Opens

A dialog window will appear prompting you to enter information about the new entry.

📷 [INSERT SCREENSHOT: sdd_metadata_new.png]

---

## Filling in the Metadata Form

### Source Selection Section

| Field | Description | Required |
|-------|-------------|----------|
| **Applicable Domain** | Select RA or FMS | Yes |
| **Module** | Select UC or PI | Yes |
| **Source** | Enter the data source identifier | Yes |
| **Vendor** | Enter the vendor name | Yes |
| **Vendor Version** | Enter the vendor version | Yes |
| **Source Name** | Enter a descriptive name for this source | Yes |

### Configuration Section

| Field | Description | Required |
|-------|-------------|----------|
| **Integration Server** | Enter the integration server identifier | Yes |
| **Phase** | Enter the phase number | Yes |
| **Instance** | Enter the instance identifier | Yes |
| **Control Points** | Enter control points configuration | Yes |
| **Loading Flow** | Enter the loading flow identifier (must start with "ld_") | Yes |
| **Data Table** | Enter the data table name | Yes |
| **Applicable Modules** | Enter the applicable modules | Yes |

### Request Information Section

| Field | Description | Required |
|-------|-------------|----------|
| **Request ID** | Enter the request identifier number | Yes |
| **Status** | Enter the current status | Yes |
| **LLD Request Version** | Enter the LLD request version number | Yes |
| **LLD Request Date** | Select the LLD request date | Yes |
| **LLD Status** | Enter the LLD status | Yes |

### Notes Section

| Field | Description | Required |
|-------|-------------|----------|
| **Notes** | Enter any additional notes about this entry | No |

---

## Saving the Entry

### Step 1: Review Your Information
Ensure all required fields are filled in correctly.

### Step 2: Click Save
Click the **Save** button to create the entry.

### Step 3: Entry Appears in Table
The new entry will appear in the metadata table on the main window.

---

## After Creating an Entry

Once you have created an entry, you can:

| Action | Description |
|--------|-------------|
| **Create Loading Rule** | Add a loading rule to define field mappings |
| **Create Layout** | Add a layout to define the data structure |
| **Edit Entry** | Modify the metadata information |
| **Delete Entry** | Remove the entry if no longer needed |

---

## Common Mistakes to Avoid

| Mistake | How to Avoid |
|---------|--------------|
| **Missing required fields** | Fill in all fields marked as required |
| **Invalid Loading Flow format** | Ensure Loading Flow starts with "ld_" |
| **Duplicate entries** | Check the table before creating new entries |

---

## Next Steps

- [Editing Entries](03_Editing_Entries.md) — Learn how to modify existing entries
- [Loading Rule Editor](04_Loading_Rule_Editor.md) — Learn how to create loading rules

---

**← [Back to SDD Overview](01_Overview.md)**
