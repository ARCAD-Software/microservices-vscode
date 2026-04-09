# Code Extraction Analysis

Code extraction analysis evaluates the impact of extracting a portion of code to ensure reusability while maintaining functional consistency.  
It identifies additional necessary code segments, determines which fields should be parameters or local variables, and simulates both the extracted and modified original code.  
The analysis is limited to the source itself, focusing on subroutines and ensuring that all referenced subroutine content is included.

## Extraction Analysis View

The Extraction Analysis View provides a comprehensive visibility into your extraction analysis with enhanced field organization.

### View Components

The extraction analysis view now displays the following sections:

#### Parameter Field
The Parameter field displays parameters required for the extracted procedure.

| Information Displayed |
|---|
| Parameter names |
| Parameter types |
| Parameter keywords (VALUE, CONST, RETURN) |
| Parameter order and sequence |

#### Local Field
The Local field displays local variables that remain within the extracted code.

| Information Shown |
| --- |
| Local variable names |
| Variable types |
| Variable scope and usage |
| Initial values (if applicable) |

#### Extraction Files
The Extraction Files section lists all the source files involved in the extraction.

| Information Shown |
| --- |
| Source file names |
| File types |
| File locations |
| Associated library information |

#### Code to be Extracted
The Code to be Extracted displays the actual code sections selected for extraction.

| Information Shown |
| --- |
| Line numbers |
| Code segments |
| Code structure |
| Comments and documentation |

#### External Call View
The External Call view displays external calls and dependencies.

| Information Shown |
| --- |
| External program/procedure calls |
| External data references |
| Call types |
| Dependency relationships |
| Open External Call Configuration (direct access to configure external call settings) |

### Accessing the Extraction Analysis View

**Step 1** From the **Rules** node, expand the **Extraction** section and right-click on an extraction analysis.

**Step 2** click the **Properties** option to open the detailed analysis view.

**Step 3** Review the organized sections. Follow the subsequent review process:

1. Examine the parameter requirements,
2. Review the local field definitions,
3. Check the extraction files involved,
4. Analyze the code to be extracted, and
5. Review the external call configuration.

**Result** The Extraction Analysis view is displayed and you have comprehensive visibility into all aspects of your extraction analysis.

### Renaming Extractions

The **Rename Extraction** feature allows you to update extraction descriptions for better organization and tracking.

**Step 1** From the **Extraction** or the **Externalization** section in the **Rules** node, right-click on an extraction analysis.

**Step 2** Select the **Rename** option from the context menu.

**Step 3** Enter a new descriptive name for your extraction.

**Step 4** Press **Enter** to confirm.

**Result** Your extraction is renamed with the updated description for better tracking and organization.

### Simulated Procedure

The extraction analysis includes a simulated procedure to help validate the result before externalization.

This simulation allows you to compare the code before and after extraction, with a detailed view of how the structure is modified and how parameters are passed to the new procedure. It also highlights variable scope to demonstrate how data remains accessible in both contexts.

By providing this preview, the simulation helps ensure functional consistency and lets you confirm that the extraction behaves as expected before applying the changes.
