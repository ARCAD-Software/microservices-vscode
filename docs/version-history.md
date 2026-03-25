# Version History - ARCAD Transformer Microservices

Complete version-wise feature documentation for ARCAD Transformer Microservices for VSCode.

> [!NOTE]
> **Compatibility Information**  
> Version 1.0.3 is compatible with V26 Server and later releases.

---

## Version 1.0.3 (Current Release)

### Overview

Version 1.0.3 represents a significant enhancement to ARCAD Transformer Microservices, introducing new features and improvements across connection management, code analysis, macro operations, and externalization workflows.

---

### Feature Categories

#### 1. Connection & Configuration Management

#### OSGI File Configuration (NEW)
- **New Entity**: `Microservices.ccsid`
- **Purpose**: Manages character set identifier settings for microservices connections
- **Level**: Application level
- **User Benefit**: Centralized connection settings management across all rules and extractions
- **Location**: Application node in rule configuration

#### License Management (ENHANCED)
- **Temporary Licenses**: Support for evaluation and trial licenses with expiration tracking
- **Permanent Licenses**: Long-term production license support
- **Feature**: Unified license management interface showing both license types
- **User Benefit**: Better visibility into license status and planning

---

#### 2. Code Analysis & Similarity Enhancements

#### Pseudocode Generation (IMPROVED)
- **Previous Behavior**: Optional pseudocode generation for each similarity match (yes/no choice)
- **Current Behavior**: Automatic pseudocode generation when needed for enhanced analysis
- **Wide Scope Support**: Enables multiple code similarity executions with broader matching capabilities
- **Pre-Requirement**: Pseudo code must be generated before performing code similarity searches
- **Accessibility**: "Generate Pseudo Code" icon available in Code Similarity Tab (top-right corner)
- **User Benefit**: Streamlined workflow with automatic handling of pseudocode generation

#### Code Similarity Execution History
- **New Structure**:
  - **Code Similarity Node**: Parent container for all similarity operations
  - **Code Similarity History**: Track all similarity executions
  - **Per-Execution History**: Detailed history for individual analysis runs
- **Features**: Each execution maintains complete history for audit and review
- **User Benefit**: Complete traceability of all similarity searches and results

#### Code Similarity Level Checking
- **New Capability**: Check/uncheck individual components in similarity results
- **Selective Matching**: Fine-grained control over which similarities to consider
- **Batch Operations**: "Check Out All" action available for specific similarity matches
- **User Benefit**: More control over which matched components to process

#### Audit SQL and RPGLE Source Members
- **Enhanced Feature**: Improved auditing of SQL and RPGLE source code
- **Application**: More comprehensive code analysis and documentation
- **User Benefit**: Better understanding of code dependencies and impacts

---

#### 3. Extraction Analysis Enhancements

#### Extraction Analysis View Redesign
The extraction analysis view now provides organized sections with enhanced visibility:

**New View Components:**
- **Parameter Field** - Shows all required parameters with types and keywords
- **Local Field** - Displays local variables within the extracted code
- **Extraction Files** - Lists all source files involved in the extraction
- **Code to be Extracted** - Displays actual code sections with line numbers
- **External Call View** - Shows external dependencies and call relationships

#### Open External Call Configuration
- **New Option**: Direct access to external call configuration
- **Accessibility**: From the External Call View section
- **User Benefit**: Quick configuration of external call settings without navigation

#### Rename Extraction Feature
- **Capability**: Update extraction descriptions for better organization
- **Scope**: Available for both successful and failed extractions
- **User Benefit**: Better tracking and identification of extraction analyses

#### Simulated Procedure
- **Enhanced Feature**: Improved simulation of extracted procedures
- **Validation**: Shows code state before and after extraction
- **Parameter Simulation**: Demonstrates parameter passing behavior
- **Variable Scope**: Shows variable accessibility in both contexts
- **User Benefit**: Verify extraction correctness before externalization

---

#### 4. Macro Commands Explorer Enhancements

#### Library Management at Application Level
- **New Level**: Application-level library configuration
- **Common Libraries**: Support for libraries like `ARCAD_ENG`
- **Features**:
  - Add library lists from Application node
  - Remove library lists with confirmation
  - Centralized management across all users
- **User Benefit**: Better organization of macro commands

#### Enhanced Macro Filtering
- **All Macro Commands**: Complete list of all available macros
- **Favorites View**: 
  - Shows TMS-related macros automatically
  - User-marked favorite macros
  - Quick access without scrolling
  - Perfect for TMS-only operations
- **User Benefit**: Faster access to frequently used macros

#### Macro Definition Viewing
- **New Method**: Double-click to view macro definitions
- **Existing Method**: Right-click > Open Macro Definition
- **Output**: JSON format showing:
  - Macro ID and name
  - Description and definition details
  - Parameters and configuration
  - All macro properties
- **User Benefit**: Quick definition access with multiple methods

#### Macro Execution History Tracking
- **Tracking Level**: Instance-level tracking of macro executions
- **Visibility**: View under Application node
- **Indicators**:
  - Successful executions (checkmark/success icon)
  - Failed executions (error icon)
  - Execution count
  - Last execution timestamp
- **Details Available**:
  - Execution date and time
  - Execution duration
  - Output results
  - Errors and warnings
- **User Benefit**: Complete audit trail of all macro executions

---

#### 5. Externalization Improvements

#### Service Program Selection
- **Previous**: Limited to creating new SRVPGM bindings
- **Current**: Support for both creating new and selecting existing Service Programs
- **Configuration**:
  - Choose between "Create New" or "Use Existing"
  - Select from available SRVPGM objects
  - Match selection to externalization requirements
- **Binding Type Support**:
  - `PGM` - Program type binding
  - `SRVPGM` - Service Program binding
- **User Benefit**: 
  - Reuse existing service programs
  - Reduce code duplication
  - Simplified binding management

#### Enhanced Binding Configuration
- **Full Control**: Complete binding object configuration
- **Options**:
  - Bind Service Program with flexibility
  - Choose from existing or new options
  - Simplified service program management
- **User Benefit**: More flexible externalization workflows

---

#### 6. User Experience Improvements

#### Comprehensive Documentation
- **Version Markers**: Clear indication of V1.0.3 features throughout documentation
- **User Perspective**: All features documented from user's point of view
- **Step-by-Step Guides**: Detailed instructions for each feature
- **Practical Examples**: Real-world usage scenarios (e.g., ARCAD_ENG library)

#### Better Feature Organization
- **Consistent Structure**: Similar features grouped logically
- **Version Information**: Clear V1.0.3 marking on new/enhanced features
- **Navigation**: Easy access to related features
- **Cross-References**: Links between related documentation

---

### Summary of User-Facing Changes

### What's New
✅ OSGI configuration with Microservices.ccsid entity  
✅ Dual license type management (Temporary/Permanent)  
✅ Automatic pseudocode generation for code similarity  
✅ Enhanced extraction analysis view with 5 new field sections  
✅ External call configuration direct access  
✅ Rename extraction functionality  
✅ Application-level library management  
✅ Enhanced macro filtering with TMS support  
✅ Double-click macro definition access  
✅ Execution history tracking for macros  
✅ Service program selection in externalization  

### What's Improved
🔄 Code similarity execution history tracking  
🔄 Macro command organization at Application level  
🔄 Externalization configuration options  
🔄 Extraction analysis presentation  
🔄 Code analysis capabilities  

---

### Documentation References

For detailed information on specific features in Version 1.0.3, refer to:
- [Rules Management](rule.md) - OSGI and License configuration
- [Code Similarity](code-similarity.md) - Pseudocode generation and similarity analysis
- [Extractions](extractions.md) - Extraction analysis views and features
- [Macro Commands](macro-commands.md) - Macro management and execution
- [Externalization](externalizations.md) - Service program selection and binding

---

## Previous Versions

[Earlier version information would be added here as needed]

---

## Ready for Future Versions

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

