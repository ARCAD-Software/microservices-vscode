
## Deploy a Web Service

The Web services management functionality offers a centralized management approach to simplify both generation and deployment processes of REST web services for ILE programs or services programs generated with ARCAD Transformer Microservices.

By taking advantage of several pieces of data generated during the process of externalizing procedure, ARCAD Transformer Microservices predefines a configuration of the appropriate web service to be created.

---

## Web Services Management

Web Services management in ARCAD Transformer Microservices uses **QShell commands** from the IBM i Integrated Web Services server.  
These commands, located in the directory `/QIBM/ProdData/OS/WebServices/bin`, are executed by the AFS server.

The following commands are used:

- `getWebServiceProperties.sh` – Retrieves web service properties.
- `installWebService.sh` – Installs web services.
- `listWebServices.sh` – Lists deployed web services.
- `startWebService.sh` – Activates stopped web services.
- `stopWebService.sh` – Deactivates active web services.
- `uninstallWebService.sh` – Removes web services.

Web services managed by ARCAD Transformer Microservices can be accessed and managed from two locations:

- **ARCAD-Microservices Explorer View**: expand the **Web Server** hosting the web services to view and manage them.  
    ![Web service list](_media/tms-servernode-webservices-list.png)

- **Web Services (List)**: located within each **Opened Version** under the **Development Version**.  
    ![Web service list](_media/tms-versionnode-webservices-list.png)

> [!Warning]  
> The system exclusively supports ILE objects, specifically ILEPGM and ILESRVPGM, created by ARCAD Transformer Microservices.

> [!NOTE]   
> This feature is limited to management actions pertinent to ARCAD Transformer Microservices functionalities.  
Additionally, certain operations may experience minor delays.

---

## Deploying a Web Service

Deploying a web service in ARCAD-Transformer Microservices involves a structured process that ensures efficient management and deployment.

<details>
<summary><strong>Step-by-step: Deploy a Web Service</strong></summary>

**Step 1** Select an **Entry Point**  
Select either:
   - an ILE object type ILEPGM or ILESRVPGM created by Transformer Microservices.  
       ![Deploy Webservice from Component](_media/tms-deploy-webservice-component.png)
   - or an extraction that has been successfully externalized.  
       ![Deploy Webservice from Extraction](_media/tms-deploy-webservice-externalization.png)

**Step 2** Right-click on **ARCAD Transformer Microservices** and click the **Deploy as Web Service** option.  
The system runs the `AAPYWEBATR` command to generate a PCML file in the `/transformer/microservices/pcml` directory.  
This ensures that PCML files are dynamically stored based on environment settings using the `AWRKENVIFS` command. The system also determines which module to insert `PGMINFO(*PCML) INFOSTMF(<IFS_directory>)` into the RPG source code.

**Step 3** Configure the **REST** and **General Attributes**. Use the assistant to fill in all the necessary fields.

**Step 4** Click **Finish** to complete the web service creation.  
A corresponding entity is added, becoming the primary interface for future interactions.  
The `.pcml` and `.properties` files will be added to your development version.

> [!NOTE]  
> The generated properties file adheres to IBM's syntax, allowing it to be used directly with IBM QShell.

</details>

### Configuring the URI Path

Each input parameter can be edited and must follow these rules:

**Path Parameters**
- Must be declared first in the **URI path template for the resource** field.
- Each input parameter must match an existing identifier.

**Query Parameters:**
- Must be defined with both identifier and default value.

> [!NOTE]  
> Auto-completion of the URI is provided to showcase its full syntax.

---

## Starting or Stopping a Web Service

<details>
<summary><strong>From the ARCAD Microservices View</strong></summary>

**Step 1** Select the web service from the inline menu to expand the Web Server.

**Step 2** Start or Stop the Web Service.  

![Start/Stop Web service](_media/tms-webservice-start.png)

**Step 3** Use the **Refresh** icon in the View Toolbar to Refresh the view.

**Result**  The server is successfully started or stopped.
</details>

<details>
<summary><strong>From the Version Web Services View</strong></summary>

**Step 1** Expand the **Web Services** node under your **Opened Version**.

**Step 2** Select a web service and choose **Start** or **Stop** from the inline menu.  

![start stop webservice](_media/tms-webservice-start.png)

**Step 3** Click **Refresh** in the View Toolbar.

**Result**  The server is successfully started or stopped.
</details>

---

## Updating a Web Service

You should update the web service if:
- the procedure interface has changed, or
- the REST attributes in the `.properties` file have changed.

<details>
<summary><strong>From the ARCAD Microservices View</strong></summary>

**Step 1** Expand the Web Server and right-click the web service.

**Step 2** Select the Update option.

![Redeploy web service](/_media/tms-redeploy-webservice.png)

**Step 3** Specify the Updated Files** (`.properties` and `.pcml`)

Click **Finish** to complete the update.
</details>

<details>
<summary><strong>From the Version Web Services View</strong></summary>

**Step 1** Expand the **Web Services** node under your **Opened Version**.

**Step 2** Right-click on the web service and select the **Update web service** option.  

![Redeploy web service](/_media/tms-versionnode-redeploy-webservice.png)

**Step 3** Specify the updated `.properties` and `.pcml` files.

![Redeploy web service](/_media/tms-redeploy-webservice-panel.png)

Click **Save** to complete the process.

</details>

---

## Deleting a Web Service

> [!WARNING]  
> Deleted web services cannot be recovered.  
All references from your system are removed except the `.pcml` and `.properties` files.

<details>
<summary><strong>From the ARCAD Microservices View</strong></summary>

**Step 1** Expand the **Web Server** node and right-click the web service.

**Step 2** Select the **Delete web service** option.  

![Delete web service](/_media/tms-delete-webservice.png)

**Step 3** Click **OK** to confirm and refresh the view.

</details>

<details>
<summary><strong>From the Version Web Services View</strong></summary>

1. Expand the **Web Services** node under your **Opened Version**.

2. Right-click on the web service and select **Delete web service**.  
   
![Delete web service](/_media/tms-version-delete-webservice.png)

**Step 3** Click **OK** to confirm and refresh the view.

</details>

---

## Viewing Web Serverice Properties

<details>
<summary><strong>From the ARCAD Microservices View</strong></summary>

**Step 1** Expand the **Web Server** node and right-click the web service.

**Step 2** Select the **Properties** option.  

![Web service properties](/_media/tms-servernode-webservice-properties.png)

**Step 3** Click **OK** to confirm and refresh the view.

</details>

<details>
<summary><strong>From the Version Web Services View</strong></summary>

**Step 1** Expand the **Web Services** node under your **Opened Version**.

**Step 2** Right-click on the web service and select the **Properties**option.  

![Web service properties](/_media/tms-versionnode-webservice-properties.png)

**Step 3** Click **OK** to confirm and refresh the view.

</details>

---

## Properties

![Web service properties](/_media/tms-webservice-properties-panel-view1.png)
![Web service properties](/_media/tms-webservice-properties-panel-view2.png)

---

## Swagger

![Web service properties](/_media/tms-webservice-properties-swagger.png)

>  **Reference**  
> For more information, refer to the [Integrated Web Services Server Administration and Programming Guide](https://www.ibm.com/docs/en/i/7.4?topic=guide-integrated-web-services-server-administration-programming).

