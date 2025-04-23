# Code Similarity Execution

In ARCAD Transformer Microservices, **Code Similarity** refers to analyzing a portion of code to identify similar code blocks within a specific project or an existing extraction.

Each similarity execution displays detailed results to help you review the identified matches.

You can access these analyses from:

- The **Code Similarity** node under the **Projects** node.
- The **Execution History** view by right-clicking an extraction in the **Extraction** or **Externalization** node of the **Rules** node.

![Project View](_media/tms-code-similarity-history-projectview.png)  

![Extraction View](_media/tms-code-similarity-history-extractionview.png)

### Execution History

![Execution History](_media/tms-code-similarity-execution-history.png)

Results appear in the **Microservices Code Similarity Result** view, which summarizes key details where similar code is found.

#### Execution Result

![Execution Result](_media/tms-code-similarity-execution-result.png)

- Component name, object type, application, environment, and version
- Start and end lines of the similar code block

From the **Similarity Analysis Result**, you can also initiate a new **Code Similarity** search or perform an **Extraction Analysis**.

> **Reference**:  
> For more information about the process behind the code similarity search works, refer to the [Principles of a Code Similarity](code-similarity-principles.md) documentation.

---

## Launching a Code Similarity Analysis From Component

### Step 1: Open the Component

Open your RPG component from the repository, then select the code block you want to search for similarities.

> ⚠️ **IMPORTANT**:  
> Code Similarity can be executed at the *Repository* level.  
> Code Similarity can be executed only CHECKEDOUT and UPDATED components in Version.

### Step 2: Access the Context Menu

Right-click and choose:  
**ARCAD Transformer Microservices > Search for similar codes**

![Search Component View](_media/tms-searchcode-similarity-componentview.png)  

![Search View](_media/tms-searchcode-similarity-view.png)

### Step 3: Configure Parameters

Fill out the **Code Similarity** settings:

- **Project**: Select an ARCAD Transformer Microservices Project from the dropdown. If none exists, click **New Project** to create one.
- **Minimum Similarity Match (%)**: Set the similarity threshold (1–100).
  > [!TIP]  
  > A 50% match means a 10-line block must share at least 5 lines with another block to be flagged as similar.

- **Minimum Components Found**: Set how many components must include similar code (1–100).
  > [!TIP]  
  > If set to 5, results are shown only when similar blocks are found in five or more components.

- **Load Pseudocode**: Choose whether to load generated pseudocode during the process.

Click **Enter** to launch the analysis.
## Launching a Code Similarity Analysis From Existing Extraction

> ⚠️ **IMPORTANT**:  
> Code Similarity can be executed at the *Repository* level.  
> Code Similarity can be executed only on CHECKEDOUT and UPDATED components in Version.

To search for similar code blocks from an existing extraction analysis:

1. Expand the **Extraction** or **Externalization** node.
2. Select an extraction analysis.
3. Right-click the analysis and choose:  
  **Code Similarity > Search for similar code**

![Code Similarity Option](_media/tms-codesimilarity-extractionview.png)

---

## Working with Code Similarity Results

### Navigating Results

After the search completes, you can view and compare pseudocode by:

1. Right-clicking a match in the **Code Similarity Results** view
2. Selecting **Show Compared Pseudocode**

This opens a comparison panel:

![Compare Pseudocode](_media/tms-code-similarity-show-pseudocode.png)  

![Compare Editor](_media/tms-code-similarity-compare-pseudocode.png)

- Left panel: **Source code**
- Right panel: **Compared code**

You can reopen a result by right-clicking and selecting **Open**, or re-execute it with **Execute**.

![Execute Again](_media/tms-code-similarity-execute-extractionview.png)  

![Open Result](_media/tms-code-similarity-open-extractionview.png)

### Launching Additional Searches

To run another similarity search based on current findings:

- Right-click a match in the results view
- Select **Search for Similar Codes**

![New Search](_media/tms-code-similarity-execute-extraction.png)

### Running an Extraction Analysis

You can also perform an **Extraction Analysis**:

- Right-click a match in the results
- Choose **Analyze for Extraction**

![Analyze](_media/tms-code-similarity-execute-extraction.png)

> **Reference**:  
> For more information, refer to the [Extraction Analysis](analyze-code.md) for more details documentation.

---

## Deleting a Code Similarity Search

> [!WARNING]  
> Deleting a similarity search is irreversible.

To delete:

1. Expand the **Project** node > **Code Similarity**
2. Right-click a similarity and choose **Remove**

![Delete from Project View](_media/tms-code-similarity-delete-projectview.png)

To delete from an extraction view:

1. Expand the **Extraction** node
2. Right-click > **Code Similarity** > **Execution History**
3. Right-click a result and select **Remove**

![Delete from Extraction View](_media/tms-code-similarity-delete-extractionview.png)
