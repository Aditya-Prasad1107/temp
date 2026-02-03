# Frequently Asked Questions

This page answers common questions about the NOVA Automation Suite.

---

## General Questions

### What is NOVA?

NOVA (Next-generation Orchestration via Versatile Automation) is a platform developed by Mobileum to automate RAID configuration tasks. It includes tools for PI and UC automation as well as SDD management.

---

### Who should use NOVA?

NOVA is designed for team members who need to:

- Configure data pipelines in RAID
- Create validations and dashboards
- Manage System Design Documents
- Automate repetitive RAID configuration tasks

---

### What are the system requirements?

| Requirement | Details |
|-------------|---------|
| Operating System | Windows 10 or later |
| Browser | Google Chrome (for RAID automation) |
| Network | Access to your organisation's RAID portal |

---

### How do I get access to NOVA?

Contact your team lead or IT department to request access to the NOVA Automation Suite.

---

## NOVA Launcher Questions

### Can I run multiple tools at the same time?

Yes, you can launch multiple tools from the NOVA Launcher. Each tool runs independently.

---

### Why does a console window appear?

The console window displays progress messages and logs from the automation tools. This is normal and helps you monitor what the application is doing.

---

### How do I close all running tools?

Click the **Exit** button on the NOVA Launcher. If tools are running, you will be asked to confirm. Click **Yes** to close all tools and exit.

---

## SDD Automation Tool Questions

### What is a metadata entry?

A metadata entry is a record that stores all information about a specific data source configuration, including source details, loading rules, layouts, and version information.

---

### What is the difference between Current Version and Finalized Version?

| Version Type | Description |
|--------------|-------------|
| **Current Version** | The version you are currently working on |
| **Finalized Version** | A version marked as ready for production use |

---

### Why does the tool remember my last folder?

The SDD Automation Tool caches your last selected folder to make your workflow faster. You do not need to navigate to the same folder each time you use the tool.

---

### What happens if I delete an entry?

Deleting an entry removes the metadata record. However, the associated loading rule and layout files remain in the folder. You may need to delete those files manually if no longer needed.

---

### What file formats can I use for layouts?

| Format | Description |
|--------|-------------|
| **ASN1** | ASN.1 grammar format |
| **XML** | XML grammar/schema format |
| **JSON** | JSON schema format |
| **DSV** | Delimited values (requires Excel file) |

---

### Why is the Consolidate SDD button disabled?

The button is disabled when:

- No destination folder is selected
- No metadata entries exist

Create at least one entry to enable the button.

---

### What is included in the consolidated report?

The consolidated SDD report includes:

- Summary of all entries
- Loading rules (one sheet per entry)
- Layouts (one sheet per entry)
- Metadata information

---

## Automation Suite Questions

### What is the difference between PI and UC modules?

| Module | Purpose |
|--------|---------|
| **PI (Platform Integrity)** | Focused on inter-system and intra-system validations |
| **UC (Usage Control)** | Focused on control points, trending, and mismatch validations |

---

### How do I get the input templates?

Click the **Download Templates** button on the module card in the Automation Suite. Templates are saved to your Downloads folder.

---

### Do I need to run operations in a specific order?

Yes, some operations depend on outputs from previous operations. Follow the recommended workflow order:

1. Entity creation
2. Formats and streams
3. Bindings
4. Validations
5. Dashboards

---

### Can I abort a running operation?

Yes, click the **Abort** button while an operation is running. The operation will stop.

---

## RAID Configuration Questions

### Why does Chrome open when I use RAID automation?

The RAID automation feature uses Chrome to interact with the RAID portal. This is how the tool automates the portal configuration.

---

### Is my password stored securely?

Your RAID credentials are stored locally in a configuration file within your destination folder. They are not transmitted over the network except when logging into the RAID portal.

---

### What should I do if RAID automation fails?

1. Verify your credentials are correct
2. Check that the RAID portal is accessible
3. Ensure your network connection is stable
4. Try running the automation again
5. Contact support if the issue persists

---

### Can I use RAID automation with multiple environments?

Yes, update the RAID Portal URL in the RAID Config settings to switch between environments (Development, Test, Production).

---

## Troubleshooting Questions

### Where can I find error logs?

Error messages and progress logs appear in the console window. You can copy this text for troubleshooting.

---

### Who do I contact for support?

Contact the Mobileum NOVA support team or your team lead for assistance with issues not covered in this documentation.

---

### How do I report a bug?

To report a bug:

1. Note the exact steps to reproduce the issue
2. Take screenshots of any error messages
3. Note the version of NOVA you are using
4. Contact the support team with this information

---

## Version Questions

### How do I check which version of NOVA I am using?

The version number is displayed in the NOVA Launcher header and in the footer of each tool.

---

### How often is NOVA updated?

Updates are released periodically to add new features and fix issues. Contact your IT team for information about updates.

---

**← [Back to Home](../00_Home.md)**
