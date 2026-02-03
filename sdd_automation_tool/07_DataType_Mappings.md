# DataType Mappings

This guide explains how to configure datatype mappings in the SDD Automation Tool.

---

## What are DataType Mappings?

DataType mappings define how each field's data type should be configured in the RAID system. For example:

- Text fields might be mapped to "VARCHAR"
- Number fields might be mapped to "INTEGER" or "DECIMAL"
- Date fields might be mapped to "DATE" or "TIMESTAMP"

---

## Opening the DataType Mappings Dialog

### Step 1: Ensure an Entry Exists

You need at least one metadata entry before accessing DataType Mappings.

### Step 2: Click DataType Mappings

Click the **DataType Mappings** button in the top bar.

📷 [INSERT SCREENSHOT: sdd_datatype_mappings.png]

---

## Understanding the DataType Mappings Interface

### Table Columns

| Column | Description |
|--------|-------------|
| **Field Name** | The name of the field |
| **Current DataType** | The currently assigned data type |
| **Available Options** | Dropdown to select a different data type |

### Available Data Types

Depending on your configuration, available data types may include:

| Data Type | When to Use |
|-----------|-------------|
| **VARCHAR** | Text and string fields |
| **INTEGER** | Whole number fields |
| **DECIMAL** | Decimal number fields |
| **DATE** | Date-only fields |
| **TIMESTAMP** | Date and time fields |
| **BOOLEAN** | True/false fields |

---

## Configuring DataType Mappings

### Step 1: Locate the Field

Find the field you want to configure in the table.

### Step 2: Select the Data Type

Click on the dropdown in the **Available Options** column and select the appropriate data type.

### Step 3: Repeat for All Fields

Configure the data type for each field that requires mapping.

---

## Saving DataType Mappings

### Step 1: Review Your Mappings

Ensure all fields are configured correctly.

### Step 2: Click Save

Click the **Save** button to save your mappings.

### Step 3: Confirmation

A confirmation message appears indicating the mappings have been saved.

---

## Where Mappings are Stored

DataType mappings are stored in a configuration file within your destination folder. This means:

- Mappings persist between sessions
- Mappings are specific to each destination folder
- Mappings can be shared by copying the configuration file

---

## Best Practices

| Practice | Description |
|----------|-------------|
| **Review all mappings** | Check each field's data type before saving |
| **Match source data** | Ensure data types match the actual source data |
| **Consider precision** | Use appropriate precision for decimal fields |

---

## Next Steps

- [RAID Configuration](08_RAID_Configuration.md) — Learn how to configure RAID settings
- [SDD Consolidation](09_SDD_Consolidation.md) — Learn how to generate consolidated reports

---

**← [Back to SDD Overview](01_Overview.md)**
