---
title: Local Group Policy editor
description: "Group Policy"
ms.prod: windows-server-threshold
ms.technology: manage-group-policy
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: fdf90e76-a1a2-4ad7-ad72-d09c81951e6d
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/12/2016
---
# Local Group Policy editor

>Applies To: Windows Server&reg; 2016, Windows Server&reg; 2012 R2, Windows Server&reg; 2012

Local Group Policy editor is a Microsoft Management Console (mmc) snap-in that is used to configure and modify Group Policy settings within Group Policy Objects (GPOs).

Administrators need to be able to quickly modify Group Policy settings for multiple users and computers throughout a network environment. The Local Group Policy editor provides administrators with a hierarchical tree structure for configuring Group Policy settings in GPOs. These GPOs can then be linked to sites, domains, and organizational units (OU) that contain computer or user objects.

Local Group Policy editor consists of two main sections:

**User Configuration** Holds settings that are applied to users (at sign-in and during periodic background refresh),

**Computer Configuration** Holds settings that are applied to computers (at startup and during periodic background refresh).

These sections are further divided into the different types of policies that can be set, such as Administrative Templates, Security, and Folder Redirection.

To work efficiently, administrators need to have immediate access to information about the function and purpose of individual policy settings. For Administrative Templates policy settings, Local Group Policy editor provides information about each policy setting directly in the web view of the console. This information shows operating system requirements, defines the policy setting, and includes any specific details about the effect of enabling or disabling the policy setting.

In addition, developers should be able to quickly and easily add Group Policy support to their software products. The Local Group Policy editor is designed to be extensible. The easiest way for developers to extend Local Group Policy editor for their applications is to write custom Administrative Template files that  they can add to Local Group Policy editor.

## Use the Local Group Policy editor
The following procedures explain how to open the Local Group Policy editor from the command line or as an mmc snap-in.

#### To open the Local Group Policy editor from the command line

-   On the **start** screen, click the **Apps** arrow. On the **Apps** screen, type **gpedit.msc**, and then press **ENTER**.

#### To open the Local Group Policy editor as a snap-in

1.  On the **start** screen, click the **Apps** arrow. On the **Apps** screen, type**mmc**, and then press **ENTER**.

2.  On the **File** menu, click **Add/remove Snap-in**.

3.  In the **Add or remove Snap-ins** dialog box, click **Local Group Policy editor**, and then click **Add**.

4.  In the **Select Group Policy Object** dialog box, click **Browse**.

5.  Click **This computer** to edit the Local Group Policy Object, or click **Another computer** to edit the Local Group Policy Object for a different computer. Click **Users** to edit Administrator, Non-Administrator, or per-user Local Group Policy Objects.

6.  Click **Finish**.

> [!NOTE]
> If you want to save a Local Group Policy editor console and choose which GPO opens in it from the command line:
> 
> In the **Select Group Policy Object** dialog box, select the **Allow the focus of the Group Policy Snap-in to be changed when launching from the command line** check box.

