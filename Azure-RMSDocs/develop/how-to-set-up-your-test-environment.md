﻿---
# required metadata

title: Set up the test environment | Azure RMS
description: Your rights-enabled application can be tested with different server options.
keywords:
author: bruceperlerms
manager: mbaldwin
ms.date: 04/28/2016
ms.topic: article
ms.prod: azure
ms.service: rights-management
ms.technology: techgroup-identity
ms.assetid: E480D8D6-F070-43D1-B2B0-6921459C3437
# optional metadata

#ROBOTS:
audience: developer
#ms.devlang:
ms.reviewer: shubhamp
ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom:

---

# Set up the test environment

Your rights-enabled application can be tested with different server options.

**Important**  It is a recommended best practice to test your Rights Management Services SDK 2.1 application first with the AD RMS pre-production environment against an AD RMS Server. Then, should you want your customer to have the ability to use your application with the Azure RMS Service, move to testing with that environment. For more information see, [Enable your service application to work with cloud based RMS](how-to-use-file-api-with-aadrm-cloud.md).

 

### Prerequisites

-   [Install the SDK](create-your-first-rights-aware-application.md)

Instructions

### Step 1: Set up your test environment

To test your rights-enabled application, you must run it against an RMS server that is configured for pre-production. A pre-production RMS server uses the pre-production/ISV certificate hierarchy to encrypt and decrypt files.

For more information about the AD RMS certificate hierarchy, see [Understanding certificate chains](understanding-certificate-chains.md).

There are two options available for testing your application against an RMS server:

-   **You can run your application on the 1-box AD RMS ISV environment**. If you are running Windows Server 2012, Windows Server 2008 R2, or Windows Server 2008 and have Hyper-V installed, you can deploy the 1-box AD RMS ISV environment by building a virtual machine using the AD RMS 1-box VHD. The 1-box AD RMS ISV environment provides an RMS server configured for pre-production and also has the Active Directory Rights Management Services Client 2.1 installed. Registry settings for the RMS server and client are already configured. To test your application, you run it on the virtual machine on which the 1-box environment is deployed.
-   **You can run your application against an RMS server that is configured for pre-production and that is deployed on your network**. In this case, you must also install and configure the AD RMS Client 2.1 on the computer where your application will be running. For information about how to do this, see [Configure client](how-to-configure-the-ad-rms-client-2-0.md). For information about how to deploy an RMS server and configure it for pre-production, see [Install and configure the server](how-to-install-and-configure-an-rms-server.md).

## Related topics

* [How-to use](how-to-use-msipc.md)
* [AD RMS SDK Webinar collateral download page](https://connect.microsoft.com/site1170/Downloads/DownloadDetails.aspx?DownloadID=42440)
* [Configure client](how-to-configure-the-ad-rms-client-2-0.md)
* [Install the SDK](create-your-first-rights-aware-application.md)
* [Install and configure the server](how-to-install-and-configure-an-rms-server.md)
* [Understanding certificate chains](understanding-certificate-chains.md)
 

 


