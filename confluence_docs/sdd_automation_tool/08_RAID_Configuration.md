# RAID Configuration

This guide explains how to configure RAID automation settings in the SDD Automation Tool.

---

## What is RAID Configuration?

RAID Configuration allows you to set up the parameters needed for automated RAID portal configuration. These settings include:

- Portal connection details
- Authentication credentials
- Module-specific parameters
- Automation preferences

---

## Opening the RAID Config Dialog

### Step 1: Ensure Requirements are Met

Before accessing RAID Configuration:

- At least one metadata entry must exist
- A destination folder must be selected

### Step 2: Click RAID Config Params

Click the **RAID Config Params** button at the bottom of the main window.

📷 [INSERT SCREENSHOT: sdd_raid_config.png]

---

## Understanding the RAID Config Interface

The RAID Configuration dialog is organised into sections:

### Connection Settings

| Field | Description |
|-------|-------------|
| **RAID Portal URL** | The URL of your RAID portal |
| **Username** | Your RAID portal username |
| **Password** | Your RAID portal password |

### Module Settings

| Field | Description |
|-------|-------------|
| **Module** | The module being configured (UC or PI) |
| **Environment** | Target environment (Development, Test, Production) |

---

## Configuring RAID Settings

### Step 1: Enter Connection Details

Fill in the connection settings:

1. Enter the RAID Portal URL
2. Enter your username
3. Enter your password

### Step 2: Configure Module Settings

Select the appropriate module and environment.

### Step 3: Configure Additional Options

Fill in any additional options specific to your configuration.

---

## Saving RAID Configuration

### Step 1: Review Settings

Ensure all required fields are filled correctly.

### Step 2: Click Save

Click the **Save** button to save your configuration.

### Step 3: Confirmation

A confirmation message appears indicating the settings have been saved.

---

## Using RAID Automation

Once RAID is configured, you can use it to automate RAID portal configuration:

### Step 1: Complete SDD Consolidation First

Before running RAID automation, you need to consolidate the entry. In the metadata table, locate the entry you want to configure.

### Step 2: Access via Consolidate and Configure

Click the **⋮ (More)** button on the entry row and select **Consolidate and Configure** to generate the consolidated Excel and run RAID automation.

### Step 3: Automation Begins

The automation process starts:

1. Chrome browser opens automatically
2. Navigates to the RAID portal
3. Logs in with saved credentials
4. Applies the configuration

### Step 4: Monitor Progress

A progress dialog shows the current status.

### Step 5: Completion

When finished, a success or error message appears.

---

## Aborting RAID Automation

If you need to stop the automation process:

### Step 1: Click Abort

In the progress dialog, click the **Abort** button.

### Step 2: Confirm Abort

Confirm that you want to stop the automation.

### Step 3: Process Stops

The automation stops, and the browser may close.

---

## Requirements for RAID Automation

| Requirement | Description |
|-------------|-------------|
| **Google Chrome** | Chrome browser must be installed |
| **Network Access** | Access to the RAID portal must be available |
| **Valid Credentials** | Username and password must be correct |
| **Finalized Version** | Entry must have a finalized loading rule version |

---

## Troubleshooting RAID Configuration

### Browser Does Not Open

| Cause | Solution |
|-------|----------|
| Chrome not installed | Install Google Chrome |
| ChromeDriver issue | The tool automatically manages ChromeDriver |

### Login Fails

| Cause | Solution |
|-------|----------|
| Wrong credentials | Verify username and password |
| Portal URL incorrect | Check the RAID Portal URL |
| Network issue | Check network connectivity |

---

## Next Steps

- [SDD Consolidation](09_SDD_Consolidation.md) — Learn how to generate consolidated reports

---

**← [Back to SDD Overview](01_Overview.md)**
