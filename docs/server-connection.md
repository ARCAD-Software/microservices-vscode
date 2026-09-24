# Connecting to your Server

The connection to an active server is mandatory to use the features of the Transformer Microservices extension.

**Complete Workflow**

**Step 1** Configure Microservices settings
**Step 2** Enter IBM i server details and connect to machine
**Step 3** After a successful connection, add your applications into the Microservices Extension
**Step 4** *[Optional]* Configure port and security settings

## Microservices Configuration

Before connecting to your IBM i server, you should configure your basic Microservices settings.

### Microservices Initial Setup

Once you install the ARCAD Transformer Microservices extension, you'll need to configure the initial settings.

**Key Configuration Areas:**
- Server connection parameters
- License management
- Port and connection settings

![Microservices Configuration](_media/tms-connection-configuration.png)

## IBM i Server Connection

### Connecting to IBM i Machine

Now enter your IBM i server details and establish the connection to the machine.

**Step 1:** To connect to your server, use the **IBM i** icon on the left side, then click on the **Connect to IBM i** button.

![TMS Connect to ibm i](_media/tms-connect-ibmi.png)

**Step 2:** Set the connection parameters for your IBM i machine:

**Connection Name / Host or IP Address**
- Enter the name, Host or IP address of the IBM i partition hosting the server
- Example: `192.168.1.100` or `ibmi.company.com`

**Username / Password**
- Enter a valid user login and password. Check the Save password if needed.

> [!NOTE] 
> This user must be declared on the server and will execute all operations on the IBM i side.

**Step 3:**  After entering your machine details, you can either click the **Connect** button to connect immediately, or click the **Save & Exit** button to connect later.

**Result:** You are successfully connected to the IBM i server.

The Transformer Microservices license is stored on the connected IBM i machine, so there is no need to add one within the extension.  
You can find the details in the **Product License Status** section in the primary panel view.

![TMS License](_media/tms-license.png)

Once you have successfully connected to the IBM i server, you can now add the applications you will work with in the Microservices Extension.

## Adding an Application

**Step 1:** Click the **+** button in the **Application** section of the extension.

![Add Application](_media/tms-application.png)

**Step 2:** A dialog opens showing available applications. Select one or several applications by checking their corresponding boxes.

![Application List](_media/tms-application-list.png)

**Available Applications** may include:
- `ARC_DEMO` Arcad demo applications
- `ARTEMIS` Test micro services
- `AZRCO` Arcad demo applications
- `FARIA1` Application FARIA1
- `FGRGA` FGR - GitHub Actions Tests
- `FGRIMS` FGR Transformer microservices

**Step 3:** Click **OK** to add the selected applications.

**Result:** Your applications are successfully added and appear in the **Application** section in the primary panel view of the **Transformer Microservices** extension.

![Added Applications](_media/tms-added-application.png)

### Removing an Application

Follow the subsequent steps to remove an application from your workspace:

**Step 1** Click the **— Remove Application** button.

**Step 2** Select the applications to remove from the drop-down list.

**Step 3** Click **OK** to confirm the removal.

**Result** The application(s) are removed from your workspace and will no longer appear in the Application section.

## Configure the Port Number and Security Settings

You can optionally configure an advanced port and security settings.

**Step 1** Configure Port & Security Settings

**Step 2** Click the ![Gear Icon](_media/icons/gear.svg) icon, then click the **Settings** option. The VScode settings open in a new tab.  
From the **Extensions** section, open the ARCAD-Transformer Microservices extension settings.

![Extensions](_media/tms-extensions.png)

**Step 3** Check the **Enable trace in ARCAD-Transformer Microservices output** box to populate the Output view to get the logs and trace the steps of the process.

**Step 4** Set the **Port Number** used to connect to the ARCAD-Transformer Microservices Server.  
By default, the port number used is **5265**.  

> [!NOTE] 
> It is possible to use a secure connection (**HTTPS**).
Before you do so, make sure to set the path to a local file containing the server's certificate chain in PEM format.

> [!NOTE]
> Add a `0` at the end of your port number when using HTTPS.

The **Field Usages Coloring** settings section allows you to customize the visual presentation of your returned results, enhancing clarity and differentiation for better readability.
