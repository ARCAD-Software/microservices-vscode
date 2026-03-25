# ARCAD-Transformer Microservices for VSCode extension
![https://marketplace.visualstudio.com/items?itemName=arcadsoftware.arcad-microservices](https://img.shields.io/visual-studio-marketplace/v/arcadsoftware.arcad-microservices)
![https://marketplace.visualstudio.com/items?itemName=arcadsoftware.arcad-microservices](https://img.shields.io/visual-studio-marketplace/i/arcadsoftware.arcad-microservices)

Welcome to the **ARCAD Microservices Extension for VSCode** Documentation!

![Arcad Microserviecs Extension](_media/tms-extension.png)

ARCAD Transformer Microservices is an integral tool in the process of modernizing legacy applications by honing in on specific sections of code that possess unique characteristics.

The emphasis on uniqueness in code sections allows for a gradual evolution of application architecture from monolithic to modular, paving the way for the implementation of highly relevant architectures like microservices.
Adopting a microservices architecture offers a myriad of benefits to both developers and enterprises:

For developers, the implementation of microservices architecture offers several significant advantages.  
By avoiding the accumulation of a large code base, it simplifies the maintenance and the addition of new features. It also enhances deployment processes and reduces IDE load times.  
Additionally, debugging becomes more straightforward, and tracking code dependencies is less cumbersome, facilitating smoother project workflows.

As for enterprises, it enables more frequent deliveries and shorter delivery times, allowing faster feedback cycles.  
It also enhances resource management and improves service availability, ultimately leading to a better user experience. 
Additionally, identifying and eliminating duplicate services can significantly reduce development expenses and operational management costs.

ARCAD Transformer Microservices is designed to facilitate the implementation of such architecture by providing functionalities that support the generation of microservices based on IBM i applications.

To achieve this goal, the product focuses on:
- auditing the risk associated with externalizing a selected portion of code before centralizing it,
- determining where a selected piece of code is used within an application, and
- ensuring the uniqueness of the call to centralized code within the application.
- automating the deployment of REST web services for IBM i ILE objects using IBM's Integrated Web Services Server (IWS),
- providing comprehensive iUnit testing support on successful externalization to ensure code quality and reliability.

---

## ARCAD Transformer Microservices for REST Web Services

**ARCAD Transformer Microservices** is designed to automate the deployment of REST web services for IBM i ILE objects (programs or service programs). Leveraging IBM's **Integrated Web Services Server (IWS)**, this tool simplifies the process of defining, managing, and deploying web services, enhancing productivity and minimizing manual intervention.

### Key Capabilities:

- **Automated REST Service Deployment** - Transform ILE objects into RESTful web services with minimal configuration
- **Service Definition Management** - Easily define and manage web service endpoints
- **IWS Integration** - Seamlessly integrate with IBM's Integrated Web Services Server
- **Reduced Manual Effort** - Automate deployment processes to enhance developer productivity
- **Enterprise-Ready** - Deploy production-grade web services with confidence

---

## Version History & Latest Features

### Version 1.0.3 (Current - Compatible with V26 Server)

This version introduces significant enhancements to improve the user experience and expand functionality across the ARCAD Transformer Microservices ecosystem.

> [!NOTE]
> Version 1.0.3 requires V26 Server or later for full compatibility.

#### **New Features for Users:**

##### **Connection & Configuration**
- **OSGI File Configuration** - New entity `Microservices.ccsid` added for enhanced connection management
- **Application Level Integration** - Changes now applied at the Application level for broader impact

##### **Code Analysis Enhancements**
- **Audit SQL and RPGLE Source Members** - Enhanced auditing capabilities for SQL and RPGLE source code analysis
- **Improved Pseudocode Generation** - The "Generate Pseudo Code" feature has been refined:
  - Previously: Generated pseudocode for each similarity match individually (yes/no option)
  - **Now**: Pseudocode generation is automatic when needed, with enhanced scope for multiple code similarity executions
  - Location: Available in the Code Similarity Tab (top-right icon) when opening a project

##### **Macro Commands Explorer Enhancements**
- **Library Management** - Users can now add library lists (e.g., `ARCAD_ENG`) from the Application node
- **Macro Filtering** - Two convenient views:
  - **All Macro Commands**: View complete list of all available macros
  - **Favorites**: Filtered view showing only TMS-related and favorite macros
- **Execution History** - Track macro execution history on the instance
- **Macro Definition Viewing** - Double-click any macro to view its complete definition

##### **License Management**
- **Dual License Types** - Users can now view and manage both:
  - **Temporary Licenses**
  - **Permanent Licenses**

##### **Extraction Analysis Updates**
- **Enhanced Analysis View** - Extraction Analysis View has been redesigned with new fields:
  - **Parameter Field**
  - **Local Field**
  - **Extraction Files**
  - **Code to be Extracted**
  - **External Call View**

##### **Code Similarity Enhancements**
- **Code Similarity Node Structure**
  - **Code Similarity History**: Track all similarity executions
  - **Per-Execution History**: View detailed history for each similarity analysis
- **Pre-Requirement**: Pseudo code must be generated before performing code similarity searches
- **Wide Scope Support**: Enables multiple code similarity executions with broader matching capabilities

##### **Extraction & Externalization Improvements**
- **Rename Extraction**: Update extraction names with more descriptive text
- **Simulated Procedure**: Enhanced procedure simulation capabilities
- **Code Similarity Levels**: Users can now check/uncheck components in match results
  - **Selective Matching**: Check/uncheck specific components in similarity results
  - **Batch Operations**: "Check Out All" action available for specific similarity matches

##### **External Call Configuration**
- **Open External Call Configuration** - New option to directly view and manage external call settings

##### **Externalization Enhancements**
- **Service Program Selection** - Users can now choose from existing Service Programs (SRVPGM)
  - **Previous**: Limited to creating new SRVPGM bindings
  - **Now**: Support for both creating new and selecting existing Service Programs
  - **Bind Service Program**: Full control over service program binding options

---
