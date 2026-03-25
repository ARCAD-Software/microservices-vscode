# Macro Commands Management

The **MACRO COMMANDS** feature in ARCAD Transformer Microservices provides users with an efficient way to browse, manage, and execute macro command lists directly from the VSCode explorer. This feature streamlines macro operations with a user-friendly interface and comprehensive management capabilities.

---

## Overview

The **MACRO COMMANDS Explorer** allows users to:
- ✅ Add and manage library lists
- ✅ Browse all macro commands filtered by favorites
- ✅ View macro definitions in JSON format
- ✅ Execute macros directly from the UI
- ✅ Track execution results in real-time

---

## MACRO COMMANDS Explorer

![MACRO COMMANDS Explorer](_media/tms-macro-commands-explorer.png)

---

## Workflow: Getting Started with Macro Commands

### Step 1: Add Library Lists

**From the Explorer Toolbar:**

**Step 1** Open the **MACRO COMMANDS** node in the ARCAD-Microservices explorer.

**Step 2** Click the **+ (Plus Icon)** in the explorer toolbar next to MACRO COMMANDS.

**Step 3** Select **Add Library List** from the options menu.

**Step 4** Enter the library details:
- Library name
- Library path
- Access permissions

**Step 5** Click **Save** to add the library.

**From the Context Menu:**

**Alternative Step 2** Right-click on **MACRO COMMANDS**.

**Alternative Step 3** Select **Add Library List** from the context menu.

**Result** The library list is added and available in the explorer for macro commands.

---

### Step 1b: Remove Library Lists

**From the Explorer Toolbar:**

**Step 1** Locate the library list you want to remove in the MACRO COMMANDS Explorer.

**Step 2** Click the **- ( Icon)** in the explorer toolbar next to the library.

**Step 3** Confirm the removal when prompted.

**From the Context Menu:**

**Alternative Step 2** Right-click on the library list.

**Alternative Step 3** Select **Remove Library List** from the context menu.

**Alternative Step 4** Confirm the removal.

**Result** The library list is removed from the explorer and the system.

---

### Step 2: View Macro Commands by Favorites

Once library lists are configured, the explorer displays:

**Available Views:**
- **All Macro Commands** - Complete list of all available macros (all will be visible to the user)
- **Favorites** - Filtered view showing only macro commands marked as favorites

![Favourite Macro Commands](_media/tms-favourite-macro-commands.jpg)

**Note:** Users can see all available macro commands in the **All Macro Commands** view. The **Favorites** view provides quick access to frequently used macros only.

---

### Step 3: View Macro Definition

To view the macro definition in JSON format:

**Step 1** Locate the macro command in the MACRO COMMANDS Explorer.

**Step 2** Right-click on the macro command.

**Step 3** Select **Open Macro Definition** from the context menu.

**Step 4** The macro definition displays in JSON format showing:
- Macro ID
- Name and description
- Definition details
- Parameters and configuration

---

### Step 4: Execute Macro Commands

#### Direct Execution

To execute a macro command directly:

**Step 1** Locate the macro command in the MACRO COMMANDS Explorer (preferably from **Favorites** view).

**Step 2** Right-click on the macro command.

**Step 3** Select **Execute** from the context menu.

![Macro Execute](_media/tms-macro-execute.png)

**Step 4** The system executes the macro and displays:
- Execution status
- Processing progress
- Results and output

**Result** The macro executes successfully and results are displayed.

---

### Step 5: View Macro Execution Logs

After executing a macro command, you can view detailed logs in the **ARCAD Macro Logs** panel:

**Step 1** After macro execution completes, the **ARCAD Macro Logs** panel opens automatically.

**Step 2** Review the logs displaying:
- Execution status (Success/Failed)
- Detailed execution output
- Error messages (if any)
- Processing timestamps
- Performance metrics

![ARCAD Macro Logs Panel](_media/tms-macro-output-panel.png)

**Step 3** Use the logs to:
- ✅ Verify macro execution success
- ✅ Troubleshoot any errors
- ✅ Monitor macro performance
- ✅ Track execution history

**Result** Complete macro execution details are visible in the ARCAD Macro Logs panel.

---

## Execution Results

After executing a macro command, the explorer displays:


## Library Management

### Adding Library Lists from Explorer

A library list contains macros specific to that library. To add a new library:

**Using the Plus Icon:**
1. Click the **+ (Plus Icon)** in the MACRO COMMANDS explorer toolbar
2. Select **Add Library List**=
3. Click **Save**

**Using the Context Menu:**
1. Right-click on **MACRO COMMANDS** node
2. Select **Add Library List**
3. Configure library details
4. Click **Save**

### Removing Library Lists from Explorer

To remove a library list:

**Using the Minus Icon:**
1. Locate the library in the explorer
2. Click the **- (Minus Icon)** next to the library
3. Confirm removal

**Using the Context Menu:**
1. Right-click on the library list
2. Select **Remove Library List**
3. Confirm removal

**Result** The library is removed from the explorer and system.

---

## Best Practices

- **Use Favorites:** Mark frequently used macros as favorites for quick access
- **Organize Libraries:** Keep library lists organized by functionality
- **Review Definitions:** Check macro definitions before execution
- **Monitor Results:** Track execution results for successful completion
- **Document Usage:** Keep records of macro executions for audit trails

---

## Related Features

- **[ARCAD Transformer Microservices](index.md)** - Overview
- **[Rules Management](rule.md)** - Work with extraction rules
- **[Web Services](web-services.md)** - Deploy web services