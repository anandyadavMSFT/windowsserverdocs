---
title: Running WSUS Replica Mode
ms.custom: na
ms.prod: windows-server-threshold
ms.reviewer: na
ms.suite: na
ms.technology: 
  - techgroup-management-and-automation
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: d218cd6b-3b6b-4429-913b-31d412ce3356
author: britw
---
# Running WSUS Replica Mode
A WSUS server running in replica mode inherits the update approvals and computer groups created on an administration server. In a scenario that uses replica mode, you typically have a single administration server, and one or more subordinate replica WSUS servers spread out throughout the organization, based on site or organizational topography. You approve updates and create computer groups on the administration server, which the replica mode servers will then mirror. Replica mode servers can be set up only during WSUS Setup, and if you implemented this scenario, it is likely because it is important in your organization that update approvals and computer groups are managed centrally.  
  
If your WSUS server is running in replica mode, you will be able to perform only limited administration capabilities on the server, which will primarily consist of:  
  
-   Adding and removing computers from computer groups. Computer group membership is not distributed to replica servers, only the computer groups themselves. Therefore, on a replica mode server, you will inherit the computer groups that you created on the administration server. However, the computer groups will be empty. You must then assign the client computers that connect to the replica server to the computer groups.  
  
-   Setting a synchronization schedule  
  
-   Specifying proxy\-server settings  
  
-   Specifying the update source. This can be a server other than the administration server  
  
-   Viewing available updates  
  
-   Monitoring update, synchronization, computer status, and WSUS settings on the server  
  
-   Running all standard WSUS reports available on replica mode servers  
  
## See also:  
  
-   [Windows Server Update Services &#40;WSUS&#41;](Windows-Server-Update-Services--WSUS-.md)  
  
-   [Update Management with Windows Server Update Services](Update-Management-with-Windows-Server-Update-Services.md)  
  
