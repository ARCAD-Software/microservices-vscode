---

# Version History - ARCAD Transformer Microservices

This page provides an overview of the main features and improvements introduced in each version of ARCAD Transformer Microservices for VSCode.

> [!NOTE]
> **Compatibility**  
> Version 1.0.4 is compatible with V26 Server and later releases.

---

## Version 1.0.4

### Overview

Version 1.0.4 reworks how extraction results are viewed, introduces project-level parameter naming standardization for externalization, adds the ability to create and run iUnit test cases directly from a successful externalization, and adds a guided Application / Component / Environment / Version / Web Server setup workflow directly from the TMS explorer. This release also brings general UI and stability improvements.

---

### What’s New

- Extraction results now open as lower-panel tabs instead of a sidebar tree
- Project-level parameter naming configuration for externalization (prefix, suffix, case format)
- iUnit test case creation, execution, and review directly from a successful externalization
- Guided setup for Application, Component, Environment, and Version creation from the TMS explorer
- Web Server creation now supports SSL/TLS configuration

---

### Key Changes

#### Viewing Results

##### Lower-Panel Tabs (New)
Extraction results are no longer shown inside the **Extraction Analysis Explorer** tree in the sidebar. Selecting **Show Extraction Results** now opens a row of Microservices tabs in the VSCode lower panel — **Parameter Fields**, **Local Fields**, **Code to be Extracted**, **File to Extract**, and **Program Calls** — next to Output, Debug Console, Terminal, and Ports. Each tab keeps a list on the left and its Usages (and, where relevant, I/O Runtime Paths) on the right. The underlying information is unchanged: only its presentation moved, making details easier to view side by side.

#### Externalization

##### Parameter Naming Configuration (New)
A project-level naming template can now be configured for parameters generated during externalization: a **Prefix Name**, a **Suffix Name**, and a **Case Format** (camelCase, PascalCase, UPPERCASE, lowercase, snake_case, UPPER_SNAKE_CASE). When a template is configured, the **Manage Externalization Parameters** dialog gains **Validate**, **Validate All**, and **Default** actions to apply, bulk-apply, or revert the naming convention on generated parameter names. Without a configured template, the behavior is unchanged.

#### Testing

##### iUnit Test Case Creation (New)
You can now create an iUnit test case directly from a successful externalization via **Actions > iUnit > Create Test Case** on the Rules node, then define its expected results, execute it, and review results and execution history, without leaving VSCode. 

> [!Note]
> This feature requires the ARCAD-iUnit extension.

#### Project Setup

##### Application, Component, Environment & Version Creation (New)
A guided setup workflow is now available directly from the TMS explorer: declare a new application, add components to it through a multi-step wizard, create an environment, and open a version, without leaving VSCode.

##### Web Server SSL/TLS (New)
Web server creation now includes an **Enable SSL/TLS** option with a dedicated HTTPS secure port, so secure web servers can be configured directly from the Create Web Server wizard.

> [!Note]
> TLS itself must still be configured on the IBM i side in IBM Web Administration for i.

#### General

##### UI and Stability Improvements
General user interface refinements and stability improvements across the extension, along with performance improvements to native components.

### What’s Improved

- Side-by-side visibility of parameter, local field, code, file, and call details when reviewing extraction results
- Consistency of parameter naming across externalized procedures
- Test coverage for externalized procedures, with results tracked over time
- Overall UI consistency and stability
- Performance of native components

### Documentation References

For detailed information, refer to:

- [Viewing Results](results.md)
- [Externalization](externalizations.md)
- [Application Setup](application-setup.md)
- [Web Services Servers](web-servers.md)

## Version 1.0.3

### Overview

Version 1.0.3 introduces improvements across code analysis, extraction workflows, macro management, and externalization, with a focus on automation, flexibility, and better visibility.

### What’s New

- OSGI configuration with the `Microservices.ccsid` entity  
- Dual license management (temporary and permanent)  
- Code similarity execution history tracking  
- Enhanced extraction analysis view  
- External call configuration access  
- Extraction renaming capability  
- Application-level library management  
- Enhanced macro filtering and favorites  
- Macro execution history tracking  
- Service Program selection for externalization  

### Key Changes

### Connection and Configuration

#### OSGI File Configuration (New)
New `Microservices.ccsid` entity to manage character set settings at the application level, allowing centralized configuration across rules and extractions.

#### License Management (Enhanced)
Improved license management with support for both temporary and permanent licenses, providing better visibility into license usage and status.

### Code Analysis

#### Pseudocode Generation (Enhanced)
Pseudocode generation is now handled automatically during similarity analysis, removing the need for manual activation and ensuring more consistent results. Manual generation remains available from the Code Similarity tab if needed.

#### Code Similarity History
Each similarity execution is now tracked, providing full visibility into past analyses and enabling easier audit and review.

#### Similarity Level Selection
You can now select or exclude individual components from similarity results, allowing more precise control over analysis outcomes.

#### SQL and RPGLE Auditing (Enhanced)
Improved auditing capabilities provide better insight into source code structure and dependencies.

### Extraction Analysis

#### Extraction Analysis View Redesign
The analysis view has been reorganized to improve readability and provide clearer visibility into parameters, local variables, source files, extracted code, and external calls.

#### External Call Configuration Access
External call settings can now be accessed directly from the analysis view, reducing navigation.

#### Extraction Renaming
You can now rename extraction analyses to improve tracking and organization.

#### Simulated Procedure (Enhanced)
The simulation preview allows you to compare code before and after extraction, understand parameter passing, and verify variable scope. This helps ensure the extraction behaves correctly before applying changes.

### Macro Commands

#### Application-Level Library Management
Libraries can now be managed at the application level, allowing centralized configuration and reuse across users.

#### Macro Filtering and Favorites
Improved filtering enables quick access to relevant macros, including TMS-related and user-defined favorites.

#### Macro Definition Access
Macro definitions can now be opened directly via double-click or context menu, providing quick access to configuration details.

#### Execution History Tracking
Macro executions are now tracked with status indicators, timestamps, duration, and detailed results, enabling full traceability.

### Externalization

#### Service Program Selection (Enhanced)
You can now either create a new Service Program or reuse an existing one when working with `SRVPGM` bindings. This reduces duplication and improves alignment with existing environments.

#### Binding Configuration (Enhanced)
Externalization now offers more flexible binding configuration options, simplifying Service Program management.

### What’s Improved

- Code similarity analysis consistency  
- Extraction analysis readability and validation  
- Macro command organization and access  
- Externalization configuration flexibility  

### Documentation References

For detailed information, refer to:

- [Rules Management](rule.md)  
- [Code Similarity](code-similarity.md)  
- [Extractions](extractions.md)  
- [Macro Commands](macro-commands.md)  
- [Externalization](externalizations.md)  
