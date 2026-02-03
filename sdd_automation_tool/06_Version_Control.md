# Version Control

This guide explains how to manage versions of loading rules in the SDD Automation Tool.

---

## What is Version Control?

Version control allows you to:

- Track changes to loading rules over time
- Keep a record of previous configurations
- Finalise versions that are ready for production use

---

## How Versions Work

### Version Numbers

Versions are numbered sequentially starting from 1:

- Version 1 — First version
- Version 2 — Second version (created when v1 is finalised)
- Version 3 — Third version (created when v2 is finalised)
- And so on...

### Version States

| State | Description |
|-------|-------------|
| **Current** | The version you are currently editing |
| **Finalized** | A version marked as ready for production |

---

## Viewing Version Information

In the metadata table, you can see version information for each entry:

| Column | Description |
|--------|-------------|
| **Current Version** | The version currently selected for this entry |
| **Last Finalized Version** | The most recent version marked as finalized |
| **Last Finalized Date** | When the last finalization occurred |

📷 [INSERT SCREENSHOT: sdd_version_dropdown.png]

---

## Editing a Loading Rule

When you edit a loading rule and click **Save**, the changes are saved to the current version file — the existing version is overwritten.

> [!NOTE]
> The Save button in the Loading Rule Editor does **not** create a new version. It saves changes to the current version.

---

## Switching Between Versions

You can switch between different versions of a loading rule:

### Step 1: Open the Version Dropdown

In the metadata table, click on the **Current Version** column for the entry.

### Step 2: Select a Version

Choose the version you want to work with from the dropdown list.

### Step 3: Version is Loaded

The selected version becomes the current version. You can now view or edit it.

---

## Creating a New Version (Finalising)

New versions are created through the **Finalize** action. When you finalize:

1. The current version is marked as finalized
2. A new version is created (current version + 1)
3. You continue editing in the new version

### How to Finalize and Create New Version

1. Locate the entry in the metadata table
2. Ensure you have completed your changes to the current version
3. Click the **Finalize** button on the entry row

📷 [INSERT SCREENSHOT: sdd_finalize_button.png]

4. Confirm the finalization

### What Happens After Finalizing

| Field | Update |
|-------|--------|
| **Last Finalized Version** | Set to the version you just finalized |
| **Last Finalized Date** | Set to the current date and time |
| **Current Version** | Incremented to the next version number |

> [!IMPORTANT]
> Always finalize a version before starting significant new changes. This ensures you have a record of the previous configuration.

---

## Best Practices

| Practice | Description |
|----------|-------------|
| **Finalize before major changes** | Finalize a working version before making significant modifications |
| **Review before finalizing** | Ensure configurations are correct before finalizing |
| **Use consistent naming** | Follow naming conventions for loading rules |

---

## Next Steps

- [DataType Mappings](07_DataType_Mappings.md) — Learn how to configure datatype mappings
- [SDD Consolidation](09_SDD_Consolidation.md) — Learn how to generate consolidated reports

---

**← [Back to SDD Overview](01_Overview.md)**
