# Code Extraction Analysis

Code extraction analysis evaluates the impact of extracting a portion of code to ensure reusability while maintaining functional consistency.  
It identifies additional necessary code segments, determines which fields should be parameters or local variables, and simulates both the extracted and modified original code.  
The analysis is limited to the source itself, focusing on subroutines and ensuring that all referenced subroutine content is included.

---

## Extraction Analysis View (Version 1.0.3+)

The Extraction Analysis View has been redesigned to provide comprehensive visibility into your extraction analysis with enhanced field organization.

### View Components

The extraction analysis view now displays the following organized sections:

#### **1. Parameter Field**
- **Purpose**: Displays parameters required for the extracted procedure
- **Information Shown**:
  - Parameter names
  - Parameter types
  - Parameter keywords (VALUE, CONST, RETURN)
  - Parameter order and sequence

#### **2. Local Field**
- **Purpose**: Shows local variables that remain within the extracted code
- **Information Shown**:
  - Local variable names
  - Variable types
  - Variable scope and usage
  - Initial values (if applicable)

#### **3. Extraction Files**
- **Purpose**: Lists all source files involved in the extraction
- **Information Shown**:
  - Source file names
  - File types
  - File locations
  - Associated library information

#### **4. Code to be Extracted**
- **Purpose**: Displays the actual code sections selected for extraction
- **Information Shown**:
  - Line numbers
  - Code segments
  - Code structure
  - Comments and documentation

#### **5. External Call View**
- **Purpose**: Shows external calls and dependencies
- **Information Shown**:
  - External program/procedure calls
  - External data references
  - Call types
  - Dependency relationships
  - **Open External Call Configuration**: Direct access to configure external call settings

### Accessing the Extraction Analysis View

**Step 1** From the **Rules** node, expand the **Extraction** section.

**Step 2** Right-click on an extraction analysis.

**Step 3** Select **Properties** to open the detailed analysis view.

**Step 4** Review the organized sections:
- Examine parameter requirements
- Review local field definitions
- Check involved extraction files
- Analyze the code to be extracted
- Review external call configuration

**Result** You have comprehensive visibility into all aspects of your extraction analysis.

### Renaming Extractions (Version 1.0.3+)

The **Rename Extraction** feature allows you to update extraction descriptions for better organization and tracking.

**Step 1** From the **Extraction** or **Externalization** section in the **Rules** node, right-click on an extraction analysis.

**Step 2** Select the **Rename** option from the context menu.

**Step 3** Enter a new descriptive name for your extraction.

**Step 4** Press **Enter** to confirm.

**Result** Your extraction is renamed with the updated description for better tracking and organization.

### Simulated Procedure

The extraction analysis includes simulated procedure functionality for validation.

**Features:**
- **Before Simulation**: Original code structure and state
- **After Simulation**: Modified code after extraction
- **Validation**: Ensures functional consistency before actual externalization
- **Parameter Simulation**: Shows how parameters would be passed to the extracted procedure
- **Variable Scope**: Demonstrates variable accessibility in both contexts

This simulation helps you verify that the extraction will work correctly before proceeding to externalization.
