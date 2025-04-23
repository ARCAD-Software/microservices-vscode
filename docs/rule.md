# Rules in ARCAD Transformer Microservices

In ARCAD Transformer Microservices, **Rules** represent business logic that should be extracted and reused by other components.

Each rule links to an extraction analysis associated with a business rule, enabling reuse and externalization.

> [!NOTE]
> Each rule is **imperatively** linked to a single ARCAD Transformer Microservices Project.

Rules can be accessed and managed from the **Rules** node.  
To access this, expand the **Rules** node under the **Projects** node located within both the **Repository** and **Version** nodes.

![Rule Node View](_media/tms-rule-viewnode.png)

---

## Creating a New ARCAD Transformer Microservices Rule

Follow these steps to create a new rule:

**Step 1:** Click the **Create a new rule** icon or right-click on the **Project** and choose **Create new rule** from the contextual menu.

![New Rule](_media/tms-create-rule.png)  
![New Rule from Project Node](_media/tms-create-rule-projectnode.png)

**Step 2:** Enter a unique **Name** for the new rule. This is a mandatory field.

Press **Enter** to proceed.

**Step 3:** Choose an existing **Project** from the list, or create a new one.

> **Reference:**  
> See [Creating a new ARCAD Transformer Microservices Project](project.md) for more information.

Press **Enter** to confirm.

**Result:** The new rule appears in the list under the **Rules** node.

---

## Moving an Existing ARCAD Transformer Microservices Rule

To move an existing rule to a different project, follow these steps:

### Steps to Move a Rule

1. **Initiate the Move:**
    - Click the **Move rule** icon from the inline toolbar on the rule node.

    ![Move Rule](_media/tms-move-rule.png)

2. **Select a Target Project:**
    - Choose an existing **Project** from the list.

    ![Move Rule - Select Project](_media/tms-move-rule-selectproject.png)

### Result

The rule is successfully moved and will now appear under the **Rules** node of the selected project.

---
## Working with an Extraction Analysis

### Viewing Extraction Analysis Properties

In the **Microservices Rules Editor**, each extraction analysis provides detailed insights.  
You can view:

- General execution information in the **Summary** tab
- All code parts to be extracted in the **Codes** tab
- Parameters and local fields in the **Fields** tab
- Error and warning messages in the **Errors/Warning messages** tab
- Externalization details in the **ILE Procedure** tab (visible only after externalization)

**Step 1:** From the **Extraction** section in the **Rules** node, right-click on an extraction analysis.

**Step 2:** Select **Properties** from the contextual menu.

![Extraction Properties Menu](_media/tms-extraction-properties-menu.png)  
![Extraction Properties Dialog](_media/tms-extraction-properties.png)

---

### Externalizing an Extraction Analysis

From the **Extraction** section in the **Rules** node, any successful extraction from a version can be externalized into a new ILE procedure.

![Externalization View](_media/tms-externalization-view.png)

> **Reference:**  
> Learn more in the [Externalization](externalisations.md) documentation.

---

### Launching a Code Similarity Search

You can search for similar code blocks from an existing extraction analysis:

- Right-click the analysis
- Select **Code Similarity > Search for similar code**

![Code Similarity Option](_media/tms-codesimilarity-extractionview.png)

> **Reference:**  
> For more details, visit the [Code Similarity](codesimilarity.md) documentation.

---

### Deleting an Extraction Analysis

> [!WARNING]  
> Deleted extraction analyses **cannot** be recovered.

**Step 1:** From the **Extraction** or **Externalization** section, right-click the analysis you wish to delete.

**Step 2:** Click **Remove** to confirm deletion.

![Delete Extraction Analysis](_media/tms-delete-extraction-ruleview.png)

---

## Deleting an ARCAD Transformer Microservices Rule

> [!WARNING]  
> Deleted rules **cannot** be recovered.

To delete a rule:

- Click the **Delete rule** icon next to the rule you want to remove.

![Delete Rule](_media/tms-delete-rule.png)

Click **OK** to confirm or **Cancel** to keep the rule.
