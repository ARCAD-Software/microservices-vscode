<!--## Ready for Future Versions

When Version 1.0.4 is released, it will be added as a new top-level section:

```
## Version 1.0.4 (Upcoming Release)

### Overview
[Version 1.0.4 features and updates]

### Feature Categories
[New features for 1.0.4]

### Summary of User-Facing Changes
[What's new and improved in 1.0.4]

### Documentation References
[Links to updated documentation]
```
-->
---

# Version History - ARCAD Transformer Microservices

This page provides an overview of the main features and improvements introduced in each version of ARCAD Transformer Microservices for VSCode.

> [!NOTE]
> **Compatibility**  
> Version 1.0.3 is compatible with V26 Server and later releases.

---

## Version 1.0.3 (Current Release)

### Overview

Version 1.0.3 introduces improvements across code analysis, extraction workflows, macro management, and externalization, with a focus on automation, flexibility, and better visibility.

---

## What’s New

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

---

## Key Changes

### Connection and Configuration

#### OSGI File Configuration (New)
New `Microservices.ccsid` entity to manage character set settings at the application level, allowing centralized configuration across rules and extractions.

#### License Management (Enhanced)
Improved license management with support for both temporary and permanent licenses, providing better visibility into license usage and status.

---

### Code Analysis

#### Pseudocode Generation (Enhanced)
Pseudocode generation is now handled automatically during similarity analysis, removing the need for manual activation and ensuring more consistent results. Manual generation remains available from the Code Similarity tab if needed.

#### Code Similarity History
Each similarity execution is now tracked, providing full visibility into past analyses and enabling easier audit and review.

#### Similarity Level Selection
You can now select or exclude individual components from similarity results, allowing more precise control over analysis outcomes.

#### SQL and RPGLE Auditing (Enhanced)
Improved auditing capabilities provide better insight into source code structure and dependencies.

---

### Extraction Analysis

#### Extraction Analysis View Redesign
The analysis view has been reorganized to improve readability and provide clearer visibility into parameters, local variables, source files, extracted code, and external calls.

#### External Call Configuration Access
External call settings can now be accessed directly from the analysis view, reducing navigation.

#### Extraction Renaming
You can now rename extraction analyses to improve tracking and organization.

#### Simulated Procedure (Enhanced)
The simulation preview allows you to compare code before and after extraction, understand parameter passing, and verify variable scope. This helps ensure the extraction behaves correctly before applying changes.

---

### Macro Commands

#### Application-Level Library Management
Libraries can now be managed at the application level, allowing centralized configuration and reuse across users.

#### Macro Filtering and Favorites
Improved filtering enables quick access to relevant macros, including TMS-related and user-defined favorites.

#### Macro Definition Access
Macro definitions can now be opened directly via double-click or context menu, providing quick access to configuration details.

#### Execution History Tracking
Macro executions are now tracked with status indicators, timestamps, duration, and detailed results, enabling full traceability.

---

### Externalization

#### Service Program Selection (Enhanced)
You can now either create a new Service Program or reuse an existing one when working with `SRVPGM` bindings. This reduces duplication and improves alignment with existing environments.

#### Binding Configuration (Enhanced)
Externalization now offers more flexible binding configuration options, simplifying Service Program management.

---

## What’s Improved

- Code similarity analysis consistency  
- Extraction analysis readability and validation  
- Macro command organization and access  
- Externalization configuration flexibility  

---

## Documentation References

For detailed information, refer to:

- [Rules Management](rule.md)  
- [Code Similarity](code-similarity.md)  
- [Extractions](extractions.md)  
- [Macro Commands](macro-commands.md)  
- [Externalization](externalizations.md)  
