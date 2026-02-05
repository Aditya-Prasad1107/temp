# SDD Automation Tool - Presentation Guide
## 50 Minutes | RA Domain (UC & PI)

---

# 🎤 OPENING SPEECH (~2 minutes)

> Good [morning/afternoon] everyone, and thank you for taking the time to join us today.
> 
> My name is [Your Name], and I'll be walking you through the **SDD Automation Tool** — a solution our team has developed to streamline the System Design Document workflow.
> 
> *(pause)*
> 
> Let me start with some context.
> 
> Preparing System Design Documents has traditionally been a manual and time-intensive process. Teams invest significant effort in creating field mappings, defining layouts across multiple formats, maintaining version consistency, and configuring the RAID portal. These are tasks that require precision and careful attention to detail.
> 
> *(pause)*
> 
> As the number of sources and vendors grows, so does the complexity. And with complexity comes the risk of inconsistencies, version mismatches, and configuration delays.
> 
> *(pause)*
> 
> The SDD Automation Tool was designed to address these challenges.
> 
> *(pause)*
> 
> So what does this tool offer?
> 
> It brings everything into a single interface. You can manage your metadata — all your source configurations — in one place. You can build loading rules with intelligent suggestions, so field mapping becomes faster and more consistent. You can define layouts in ASN1, XML, JSON, or DSV formats, with validation built right in — so errors are caught early. You can configure how fields map to RAID data types. You have proper version control, with clear separation between what you're working on and what's finalized for production. And when you're ready, you can consolidate everything into Excel reports and configure the RAID portal — all from the same tool.
> 
> *(pause)*
> 
> The result is a significant reduction in manual effort, with built-in safeguards to ensure accuracy.
> 
> *(pause)*
> 
> Today's session is approximately 50 minutes. We'll focus on the **Revenue Assurance domain**, covering both the **UC** and **PI** modules. By the end, you'll have a clear understanding of each feature and how it fits into your workflow.
> 
> *(pause)*
> 
> Let's begin.

---

# 📋 FUNCTIONALITY COVERAGE

---

## 1. Main Interface Overview (4 min)
**Time: 0:00 - 4:00**

| Topic | What to Cover |
|-------|---------------|
| **Top Bar** | Destination folder selector, DataType Mappings button, Column visibility toggle, Refresh button |
| **Metadata Table** | Columns: Domain, Module, Source, Vendor, Version, Source Name, Loading Rule, Layout, Current Version, Last Finalized, Actions |
| **Bottom Bar** | Create New Entry, RAID Config, Consolidate SDD, Close buttons |
| **Row Actions** | Edit, View, Delete, Finalize, More options (⋮) |

### 🔁 Section Summary & Transition

> *"To summarize the main interface:*
> 
> *The **Top Bar** is your configuration area — destination folder selection, DataType Mappings access, column visibility controls, and refresh.*
> 
> *The **Metadata Table** is the central view showing all your SDD entries with key information: Domain, Module, Source, Vendor, Version details, Loading Rule/Layout status, and version tracking.*
> 
> *The **Bottom Bar** contains the primary actions — creating entries, RAID configuration, SDD consolidation, and closing the application.*
> 
> *Each **Row** has quick actions: Edit, View, Delete, Finalize, and a More menu for additional options.*
> 
> *Keep in mind: this is your command center. Everything else we cover today originates from here.*
> 
> *Now, let's create a new entry..."*

---

## 2. Creating New Entry - Mandatory Fields (5 min)
**Time: 4:00 - 9:00**

| Topic | What to Cover |
|-------|---------------|
| **Mandatory Source Info** | Applicable Domain (RA), Module (UC/PI), Source, Vendor, Vendor Version, Source Name |
| **Mandatory Configuration** | Loading Flow — **must start with `ld_` prefix** |
| **Optional Fields** | Integration Server, Phase, Instance, Control Points, Data Table, Applicable Modules, Request Info — complete before consolidation |
| **Post-Save Prompt** | Options to create Loading Rule, Layout, or Neither |

### 🔁 Section Summary & Transition

> *"When creating a new entry, here are the essentials:*
> 
> ***Mandatory fields:*** Applicable Domain, Module, Source, Vendor, Vendor Version, Source Name, and Loading Flow.*
> 
> ***Critical requirement:*** The Loading Flow must always start with `ld_`. Without this prefix, consolidation will fail — so it's worth getting right from the start.*
> 
> ***Optional fields*** — Integration Server, Phase, Instance, Control Points, Data Table, Applicable Modules, and Request Info — can be added later, but must be complete before consolidation.*
> 
> *After saving, you'll be prompted to create a Loading Rule, Layout, or skip to neither.*
> 
> *Let's move to the Loading Rule Editor — where we define the field mappings..."*

---

## 3. Loading Rule Editor (10 min)
**Time: 9:00 - 19:00**

| Topic | What to Cover |
|-------|---------------|
| **UC Columns** | ID, Dimension/Measure indicator, Name, Mapping, Lookup Table, Comments |
| **PI Columns** | ID, Keys/Attributes indicator, Name, **SUBS, SERV, PACK, DEV** checkboxes, Mapping, Lookup Table, Comments |
| **Mapping Options Inspector** | **Three sections:** |
| | 1. **Available Mapping Expressions** — auto-suggested mappings based on context |
| | 2. **Or Enter Manually** — free-text entry for custom expressions |
| | 3. **Current Value** — displays and allows editing of current cell value |
| **Layout Reference Panel** | Toggle button to view layout alongside mapping for reference |
| **Row Operations** | Add Row, Delete Selected Rows |
| **Column Operations (PI only)** | Add Column, Reset Column |
| **Save Behavior** | Overwrites current version — **does NOT create a new version** |

### 🔁 Section Summary & Transition

> *"The Loading Rule Editor is where the core mapping work happens. Key points:*
> 
> *For **UC**, you have: ID, Dimension/Measure, Name, Mapping, Lookup Table, and Comments.*
> 
> *For **PI**, you have additional columns: **SUBS, SERV, PACK, DEV** — checkboxes that define entity applicability.*
> 
> *The **Mapping Options Inspector** has three sections: Available Mapping Expressions for suggestions, Manual Entry for custom expressions, and Current Value for viewing/editing.*
> 
> *The **Layout Reference** toggle is very useful — it lets you view the layout side-by-side while mapping, so you don't have to switch back and forth.*
> 
> *Row operations: Add Row, Delete Rows. PI also has Add Column and Reset Column.*
> 
> ***Important:*** When you click Save, it overwrites the current version. It does not create a new version. Versioning is a separate action we'll cover shortly.*
> 
> *Before we go further — what if the source or vendor you need doesn't exist yet?"*

---

## 4. Creating New Source/Vendor (3 min)
**Time: 19:00 - 22:00**

| Topic | What to Cover |
|-------|---------------|
| **Adding New Source** | Type the name directly in the metadata dialog — automatically added |
| **Adding New Vendor** | Type the name — becomes available for all entries |
| **Persistence** | New sources and vendors are persisted in the destination folder |

### 🔁 Section Summary & Transition

> *"Adding a new source or vendor is straightforward:*
> 
> *Simply type the name in the metadata dialog — no additional configuration required. It's added automatically.*
> 
> *New vendors become available across all entries. Both sources and vendors are persisted in your destination folder.*
> 
> *A small but useful feature — saves time when onboarding new data sources.*
> 
> *Now, let's look at how we define layouts..."*

---

## 5. Layout Editor (7 min)
**Time: 22:00 - 29:00**

| Topic | What to Cover |
|-------|---------------|
| **Supported Formats** | ASN1, XML, JSON (text-based entry), DSV (Excel upload with preview) |
| **JSON Validation** | Validates object/array structure, reports syntax errors with line and column number |
| **XML Validation** | Validates tag structure, reports errors with location |
| **ASN1 Validation** | Validates structure, reports errors |
| **DSV Handling** | Upload Excel file, preview data in table format |
| **Preview Other Operators** | View layouts from other sources, copy content, apply to current entry |

### 🔁 Section Summary & Transition

> *"The Layout Editor supports four formats: ASN1, XML, JSON, and DSV.*
> 
> *For **JSON** — the editor validates structure and reports syntax errors with exact line and column numbers.*
> 
> *For **XML and ASN1** — tag structure is validated with error locations provided.*
> 
> *For **DSV** — you can upload an Excel file and preview it in a table format.*
> 
> *The **Preview Other Operators** feature is particularly useful — it allows you to view layouts from other sources, copy content, and apply it to your current entry. Great for consistency across similar sources.*
> 
> *Now, let's look at DataType Mappings..."*

---

## 6. DataType Mappings (2 min)
**Time: 29:00 - 31:00**

| Topic | What to Cover |
|-------|---------------|
| **Purpose** | Define how fields map to RAID data types: VARCHAR, INTEGER, DECIMAL, DATE, TIMESTAMP, BOOLEAN |
| **UC Configuration** | 2 columns |
| **PI Configuration** | 3 columns |
| **Reset to Defaults** | Reloads mappings from source file `Data_Type_Mappings.xlsx` |

### 🔁 Section Summary & Transition

> *"DataType Mappings define how your fields translate to RAID data types — VARCHAR, INTEGER, DECIMAL, DATE, TIMESTAMP, and BOOLEAN.*
> 
> *UC has a 2-column configuration; PI has 3 columns.*
> 
> *The **Reset to Defaults** button reloads from the source `Data_Type_Mappings.xlsx` file — useful if you need to restore standard mappings.*
> 
> *Now, an important topic — versioning..."*

---

## 7. Version Control (5 min)
**Time: 31:00 - 36:00**

| Topic | What to Cover |
|-------|---------------|
| **Version States** | Current (active working copy) vs Finalized (locked, production-ready) |
| **Save Action** | Overwrites the current version — does not create a new version |
| **Finalize Action** | Locks current version, marks as finalized, creates new current version for future edits |
| **Version Dropdown** | Switch between versions to view or compare |

### 🔁 Section Summary & Transition

> *"Version Control is critical to understand:*
> 
> *There are two states: **Current** — your active working copy, and **Finalized** — a locked, production-ready version.*
> 
> ***Save*** overwrites the current version. It's your working save.*
> 
> ***Finalize*** locks the current version, marks it as finalized, and automatically creates a new current version for future edits.*
> 
> *Use the **Version Dropdown** to switch between versions for viewing or comparison.*
> 
> ***Key point:*** You must have at least one finalized version before you can consolidate. This ensures only reviewed, approved configurations go into production.*
> 
> *Let's now complete the workflow with consolidation..."*

---

## 8. Completing Metadata & SDD Consolidation (7 min)
**Time: 36:00 - 43:00**

| Topic | What to Cover |
|-------|---------------|
| **Pre-Consolidation Requirements** | Complete optional metadata: Integration Server, Phase, Instance, Control Points, Request Info |
| **Consolidation Prerequisites** | At least one finalized version, complete metadata fields, `ld_` prefix on Loading Flow |
| **Validation Checks** | Required field validation, sheet name length limits, file existence verification |
| **Output Generated** | Summary sheet + Loading Rules sheets + Layout sheets in Excel format |
| **Common Errors** | Missing source, invalid Loading Flow (no `ld_` prefix), no finalized version available |

### 🔁 Section Summary & Transition

> *"Before consolidation, ensure your metadata is complete:*
> 
> *The optional fields — Integration Server, Phase, Instance, Control Points, Request Info — should all be filled in.*
> 
> ***Prerequisites for consolidation:***
> - *At least one finalized version*
> - *Complete metadata fields*
> - *Loading Flow with `ld_` prefix*
> 
> *The tool runs validation checks: required fields, sheet name length limits, file existence.*
> 
> ***Output:*** A consolidated Excel file with Summary sheet, Loading Rules sheets, and Layout sheets.*
> 
> ***Common errors to watch for:*** Missing source name, Loading Flow without `ld_` prefix, or no finalized version.*
> 
> *Now, let's see how RAID automation ties everything together..."*

---

## 9. RAID Config & Closing (7 min)
**Time: 43:00 - 50:00**

| Topic | What to Cover |
|-------|---------------|
| **RAID Configuration** | Portal URL, user credentials, Module selection, Environment selection |
| **Consolidate and Configure** | Single action: generates Excel + triggers RAID portal automation |
| **Requirements** | Chrome browser, network access to RAID portal, at least one finalized version |

### 🔁 Section Summary

> *"For RAID Configuration:*
> 
> *You'll need to provide: Portal URL, credentials, Module, and Environment.*
> 
> *The **Consolidate and Configure** button performs both actions in sequence — Excel generation followed by RAID portal automation.*
> 
> ***Requirements:*** Chrome browser installed, network access to the RAID portal, and at least one finalized version.*
> 
> *This is where the automation delivers significant time savings — configurations that previously required multiple manual steps are now handled in a single action."*

---

# 🏁 CLOSING SPEECH (~2 minutes)

> That brings us to the end of today's demonstration.
> 
> *(pause)*
> 
> Let me briefly recap what we covered:
> 
> We started with the **Main Interface** — understanding the layout, navigation, and primary actions.
> 
> We walked through **Creating New Entries** — the mandatory fields, the importance of the `ld_` prefix, and how optional fields fit in.
> 
> We explored the **Loading Rule Editor** — the Mapping Options Inspector with its three sections, the Layout Reference panel, and the distinction between UC and PI configurations.
> 
> We covered how to add **New Sources and Vendors** on the fly.
> 
> We looked at the **Layout Editor** — supporting ASN1, XML, JSON, and DSV formats with built-in validation.
> 
> We reviewed **DataType Mappings** and the Reset to Defaults option.
> 
> We discussed **Version Control** — the critical difference between Save and Finalize, and why finalized versions are required for consolidation.
> 
> We went through **Metadata Completion** and **SDD Consolidation** — prerequisites, validation, and expected output.
> 
> And finally, we demonstrated **RAID Automation** — bringing the entire workflow together.
> 
> *(pause)*
> 
> The objective behind this tool is to streamline a process that has traditionally required significant manual effort — and to do so with built-in safeguards that help ensure accuracy and consistency.
> 
> *(pause)*
> 
> We believe this will make a meaningful difference in how teams manage their SDD workflow.
> 
> *(pause)*
> 
> I'm happy to take any questions at this point. If you'd like to revisit any specific feature or see additional details, please let me know.
> 
> *(pause)*
> 
> Thank you all for your time and attention today. We look forward to your feedback.

---

# ⏱️ TIME SUMMARY

| # | Section | Duration | End Time |
|---|---------|----------|----------|
| 1 | Main Interface | 4 min | 4:00 |
| 2 | Creating Entry | 5 min | 9:00 |
| 3 | Loading Rule Editor | 10 min | 19:00 |
| 4 | Source/Vendor | 3 min | 22:00 |
| 5 | Layout Editor | 7 min | 29:00 |
| 6 | DataType Mappings | 2 min | 31:00 |
| 7 | Version Control | 5 min | 36:00 |
| 8 | Metadata & Consolidation | 7 min | 43:00 |
| 9 | RAID + Closing | 7 min | 50:00 |
