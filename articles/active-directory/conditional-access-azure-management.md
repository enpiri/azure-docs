---
title: Manage access to Azure management with conditional access in Azure Active Directory
description: Learn about using conditional access in Azure AD to manage access to Azure management.
services: active-directory
documentationcenter: ''
author: skwan
manager: mtillman
editor: bryanla
ms.assetid: 0adc8b11-884e-476c-8c43-84f9bf12a34b
ms.service: active-directory
ms.devlang: na
ms.topic: article
ms.tgt_pltfrm: na
ms.workload: identity
ms.date: 09/22/2017
ms.author: skwan
---

# Manage access to Azure management with conditional access

Conditional access in Azure Active Directory (Azure AD) controls access to cloud apps based on specific conditions that you specify. To allow access, you create conditional access policies that allow or block access based on whether or not the requirements in the policy are met. 

Typically, you use conditional access to control access to your cloud apps. You can also set up policies to control access to Azure management based on certain conditions (such as sign-in risk, location, or device) and to enforce requirements like multi-factor authentication.

To create a policy for Azure management, you select **Microsoft Azure Management** under **Cloud apps** when choosing the app to which to apply the policy.

![Conditional access for Azure management](./media/conditional-access-azure-mgmt.png)

The policy you create applies to all Azure management endpoints, including classic Azure portal, Azure portal, Azure Resource Manager provider, classic Service Management APIs, and PowerShell.

> [!CAUTION]
> Make sure you understand how conditional access works before setting up a policy to manage access to Azure management. Make sure you don't create conditions that could block your own access to the portal.

For more information on how to set up and use conditional access, see [Conditional access in Azure Active Directory](active-directory-conditional-access-azure-portal.md).