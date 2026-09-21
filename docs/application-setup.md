# Application, Component, Environment & Version Setup

This page covers the core setup workflow for a new TMS project directly from the TMS explorer in VSCode: declaring an application, adding a component to it, creating an environment, and opening a version. For creating a web server (optionally with SSL/TLS), see [Web Services Servers](web-servers.md).

## Creating an Application

Declaring a new application accepts the following parameters:

| Parameter | Description |
|---|---|
| Application code | Mandatory, unique identifier for the new application. |
| Description | Mandatory free-text label for the application. |
| Application manager | Defaults to the current IBM i user profile. |
| ASP group | `*SYSBAS` by default. |
| Library prefix | Mandatory; used to derive the application's library names. |
| Operational libraries | Mandatory, one library per line (e.g. data, source and object libraries). |

**Step 1** In the TMS explorer, under **APPLICATION**, click the **+** icon (or right-click) and select **Declare a new Application**.

![APPLICATION node - Declare a new Application](_media/tms-app-declare-menu.png)

**Step 2** The **Declare a new Application** panel opens. Enter an **Application code** and **Description** (both required), confirm the **Application manager** and **ASP group**, then set the **Library prefix** and the **Operational libraries** — one library per line — both required.

![Declare a new Application panel - empty form](_media/tms-app-declare-panel-empty.png)

> **Example**  
> Application code = `TSTAR4`, Description = `TETS`, Application manager = `AKUMAR`, ASP group = `*SYSBAS`, Library prefix = `AN91`, Operational libraries = `AN91_DTA`, `AN91_SRC`, `AN91_OBJ`.

![Declare a new Application panel - completed form](_media/tms-app-declare-panel-filled.png)

**Step 3** Click **Create Application**.

**Result** A confirmation notification is displayed in the VSCode notification area.

![Notification - Application created successfully](_media/tms-app-declare-notification.png)

---

## Creating a Component

Creating a component walks through a guided, multi-step command that accepts:

| Parameter | Description |
|---|---|
| Component name | Mandatory identifier for the new component. |
| Component description | Optional, 50 characters maximum. |
| Type | The object type to create, chosen from a filterable list (e.g. `*BNDDIR`, `*DTAARA`, `*MSGF`, `*QMFORM`, `BND`, `CBL`, `CLLE`, `CMD`, `DSPF`, `ILEPGM`, `ILESRVPGM`, `INDEX`, `LF`, `MENU`, `PF`, `PNLGRP`, `PRTF`, `RPG`, `RPGLE`, `RPGLEINC`, `SQLMASK`, `SQLPRC`, `SQLRPGLE`, `SQLSEQ`, `SQLTRG`, `SQLUDF`, `SQLVAR`, `SYSTRG`, `TABLE`, `VIEW`). |
| Object type | For ILE types (e.g. `RPGLE`), whether the component is a `*MODULE` or a `*PGM`. |
| Source file | The source physical file the member is created in (e.g. `QRPGLESRC`). |

**Step 1** Under the application, expand **Component**, click the **+** icon next to the target library filter and select **Create Component** (as opposed to **Create Object**).

![Component node - Create Component / Create Object](_media/tms-component-create-menu.png)

**Step 2** Enter the **Component Name** (step 1 of 7).

![Component Name - empty](_media/tms-component-name-empty.png)

> **Example:** `TSTRPG`

![Component Name - filled](_media/tms-component-name-filled.png)

**Step 3** Enter an optional **Component Description**, 50 characters maximum (step 2 of 7).

![Component Description](_media/tms-component-description.png)

**Step 4** Choose the object type to create from the filterable list (step 3 of 7).

![Select a type - list](_media/tms-component-type-list.png)

![Select a type - scrolled](_media/tms-component-type-list-scrolled.png)

Typing filters the list, e.g. entering `RPGLE` narrows it to `RPGLE`, `RPGLEINC`, and `SQLRPGLE`.

![Select a type - filtered to RPGLE](_media/tms-component-type-filtered.png)

**Step 5** For ILE types such as `RPGLE`, select whether the component is a `*MODULE` or a `*PGM` (step 4 of 7).

![Select object type - MODULE or PGM](_media/tms-component-object-type.png)

**Step 6** Select the source file the member is created in, e.g. `QRPGLESRC` (step 6 of 7). The wizard steps through the remaining prompts before submitting the request.

![Select source file](_media/tms-component-source-file.png)

**Result** Once the wizard completes, a confirmation notification is displayed in the VSCode notification area.

![Notification - Component created](_media/tms-component-notification.png)

---

## Creating an Environment

Creating an environment requires an environment code and accepts the following parameters:

| Parameter | Description |
|---|---|
| Environment code | Mandatory identifier for the new environment. |
| Description | Free-text label for the environment (defaults to " environment" if left blank). |
| Library prefix | Defaults to `*DFT`, but this value is not authorized on every setup; it must be changed if creation fails. |
| Site | `*LCL` by default. |
| Environment type | e.g. `*DEV`, `*TST`. |
| Implementation type | e.g. `*EXT`, `*NRM`. |
| Delivery server | Whether the environment is usable by the Deliver Server. |

**Step 1** In the TMS explorer, right-click the **Environment** node and select **Create Environment** from the context menu.

![Environment node context menu - Create Environment](_media/tms-env-create-menu.png)

**Step 2** The **Create a new Environment** panel opens. Enter an **Environment code** (required — shown in red until filled), an optional **Description**, and adjust the **Library prefix**, **Site**, **Environment type**, **Implementation type**, and **Delivery server** as needed.

![Create a new Environment panel - empty form](_media/tms-env-create-panel-empty.png)

> **Example**  
> Environment code = `TESTENV`, Description = `TETS`, Library prefix = `AN64`, Site = `*LCL`, Environment type = `*DEV`, Implementation type = `*NRM`, Delivery server = `*NO`.

![Create a new Environment panel - completed form](_media/tms-env-create-panel-filled.png)

**Step 3** Click **Create Environment**.

**Result** A confirmation notification is displayed in the VSCode notification area.

![Notification - Environment created successfully](_media/tms-env-create-notification.png)

---

## Opening a Version

Opening a version requires selecting the target application/environment and accepts the following parameters:

| Parameter | Description |
|---|---|
| Version type | e.g. `*RELEASE`. |
| Description and Status | Free-text label and initial status (`OPEN` by default). |
| Increment | Version numbering rule, or a Custom version number when Increment is set to Custom. |
| Incremental parameters | Mode, Node version, Parent version. |
| Version type parameters | XRef level, Checkout from reference, Lock objects at checkout, Allow edits, Update XRef, Storage location. |
| Version linking parameters | Linked application and Linked version, both `*NONE` by default. |

**Step 1** Under the target environment, expand **Opened Versions**, then right-click and select **Open Version**.

![Opened Versions - right-click - Open Version](_media/tms-version-open-menu.png)

**Step 2** The **Open version** panel opens for the selected application and environment. Set the **New version** parameters (Version type, Description, Increment, Custom version, Status), the **Incremental parameters** (Mode, Node version, Parent version), and the **Version type parameters** (XRef level, Checkout from reference, Lock objects at checkout, Allow edits, Update XRef, Storage location).

![Open version panel - New version, Incremental and Version type parameters](_media/tms-version-open-panel-1.png)

Scroll down to review the **Version linking parameters** (Linked application, Linked version — `*NONE` by default), then click **open**.

![Open version panel - Version linking parameters and open button](_media/tms-version-open-panel-2.png)

**Result** A confirmation notification is displayed in the VSCode notification area, naming the application, version number, and target environment.

![Notification - version opened](_media/tms-version-open-notification.png)
