---
title: "Configure a Report Server (Reporting Services Native Mode) | Microsoft Docs"
description: Learn about additional configuration for SQL Server Report Server, which depends on options you chose during installation. 
ms.date: 06/18/2019
ms.service: reporting-services
ms.subservice: report-server


ms.topic: conceptual
helpviewer_keywords: 
  - "report server configuration"
  - "report servers [Reporting Services], configuring"
ms.assetid: ef84ce9d-9156-48e9-8073-7e0535476932
author: maggiesMSFT
ms.author: maggies
---
# Configure a Report Server (Reporting Services Native Mode)
  Depending on options you selected during installation, the Report Server might require additional configuration before you can use it. At a minimum, a report server configuration consists of the following:  
  
-   A Report Server service account (configured during installation).  
  
-   A Web service URL that provides access to the report server.  
  
-   A report server database that stores application data, reports, and other items.  
  
 Setup configures the minimum settings if you select either of the following installation options: Native mode default configuration or SharePoint integrated mode default configuration. If you installed the report server in files-only mode (this is the **Install but do not configure** option in the Installation wizard), only the service account is configured. The Web service URL and report server database must be configured after Setup is finished.  
  
It's recommended that you configure web portal so that you can grant user access to the report server and manage report server content. If you deploy a report server in SharePoint integrated mode, use the Web front end of a SharePoint server to grant access.  
  
 Additional features, such as report server e-mail and the unattended execution account, can be configured as needed. For more information, see [Manage a Reporting Services Native Mode Report Server](../../reporting-services/report-server/manage-a-reporting-services-native-mode-report-server.md).  
  
 To configure a report server, use the Reporting Services Configuration tool.  
  
## To minimally configure a report server installation  
  
1.  Start the Reporting Services Configuration tool and connect to the report server instance. For instructions, see [Report Server Configuration Manager &#40;Native Mode&#41;](../../reporting-services/install-windows/reporting-services-configuration-manager-native-mode.md).  
  
2.  Click **Web Service URL** to open the page for configuring a URL for the report server. For instructions on how to define the URL, see [Configure a URL  &#40;Report Server Configuration Manager&#41;](../../reporting-services/install-windows/configure-a-url-ssrs-configuration-manager.md).  
  
3.  Click **Database** to create the report server database. For instructions, see [Create a Native Mode Report Server Database  &#40;Report Server Configuration Manager&#41;](../../reporting-services/install-windows/ssrs-report-server-create-a-native-mode-report-server-database.md).  
  
4.  Go back to the **Web Service URL** page and click the URL to verify it works.  
  
5.  Follow the instructions in "Next Steps" to complete your deployment.  
  
## Next Steps  
 To complete your deployment, you should configure the web portal or SharePoint integration. For more information, see [Configure the web portal](../../reporting-services/report-server/configure-web-portal.md).  
  
 If Windows Firewall is turned on, the port that the report server is configured to use is most likely closed. One indication that a port might be closed is a blank page when you attempt to open the web portal from a remote client computer. For information on configuring the firewall, see [Configure a Firewall for Report Server Access](../../reporting-services/report-server/configure-a-firewall-for-report-server-access.md).  
  
 If you are using Windows Vista or Windows Server 2008, additional steps are required before you can open the web portal locally. For more information, see [Configure a Native Mode Report Server for Local Administration &#40;SSRS&#41;](../../reporting-services/report-server/configure-a-native-mode-report-server-for-local-administration-ssrs.md).  
  
 Verify your installation by creating folders, uploading items, and running reports. Follow the instructions in [Verify a Reporting Services Installation](../../reporting-services/install-windows/verify-a-reporting-services-installation.md) to verify your installation.  
  
## See also  
 [Manage a Reporting Services Native Mode Report Server](../../reporting-services/report-server/manage-a-reporting-services-native-mode-report-server.md)   
 [Configure a Firewall for Report Server Access](../../reporting-services/report-server/configure-a-firewall-for-report-server-access.md)   
 [Configure a Native Mode Report Server for Local Administration &#40;SSRS&#41;](../../reporting-services/report-server/configure-a-native-mode-report-server-for-local-administration-ssrs.md)   
 [Configure a Report Server for Remote Administration](../../reporting-services/report-server/configure-a-report-server-for-remote-administration.md)   
 [Report Server Configuration Manager &#40;Native Mode&#41;](../../reporting-services/install-windows/reporting-services-configuration-manager-native-mode.md)  
  
