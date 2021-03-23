---
title: Đặt cấu hình Azure Active Directory Pass-thông qua xác thực
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6970"
- "9003915"
ms.openlocfilehash: be993b1f22d89a92afb099937dae815dc9c09e0e
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037536"
---
# <a name="configure-azure-active-directory-pass-through-authentication"></a><span data-ttu-id="f42f1-102">Đặt cấu hình Azure Active Directory Pass-thông qua xác thực</span><span class="sxs-lookup"><span data-stu-id="f42f1-102">Configure Azure Active Directory pass-through authentication</span></span>

<span data-ttu-id="f42f1-103">Dưới đây là một số hướng dẫn để giúp bạn cấu hình xác thực chuyển qua:</span><span class="sxs-lookup"><span data-stu-id="f42f1-103">Here are some guides to help you configure pass-through authentication:</span></span>

- <span data-ttu-id="f42f1-104">**Để thiết lập Azure Active Directory Connect**: [người dùng đồng bộ hóa với hướng dẫn thư mục của bạn](https://admin.microsoft.com/AdminPortal/Home) sẽ giúp bạn đặt cấu hình việc đồng bộ hóa băm mật khẩu hoặc thông qua xác thực.</span><span class="sxs-lookup"><span data-stu-id="f42f1-104">**To set up Azure Active Directory Connect**: The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide helps you configure password hash synchronization or pass-through authentication.</span></span> <span data-ttu-id="f42f1-105">Cấu hình này cho phép người dùng đăng nhập vào email của họ và đến Active Directory tại cơ sở của bạn (bộ điều khiển tên miền) bằng cùng một mật khẩu.</span><span class="sxs-lookup"><span data-stu-id="f42f1-105">This configuration enables users to sign in to their email and to your on-premises Active Directory (domain controller) using the same password.</span></span>  <span data-ttu-id="f42f1-106">[Người dùng đồng bộ hóa với hướng dẫn thư mục của bạn](https://admin.microsoft.com/AdminPortal/Home) cũng bao gồm đăng nhập liên kết với các dịch vụ liên kết Active Directory (AD FS).</span><span class="sxs-lookup"><span data-stu-id="f42f1-106">The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide also covers federation sign-in with Active Directory Federation Services (AD FS), too.</span></span>

- <span data-ttu-id="f42f1-107">**Để thiết lập các tính năng Azure**: [hướng dẫn thiết lập Azure AD sẽ hướng dẫn](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) bạn thiết lập các tính năng trong Azure Active Directory BASIC, như quản lý Access dựa trên nhóm, đặt lại mật khẩu tự phục vụ cho các ứng dụng đám mây và ứng dụng Azure Active Directory proxy để phát hành các ứng dụng web tại cơ sở.</span><span class="sxs-lookup"><span data-stu-id="f42f1-107">**To set up Azure features**: The [Azure AD setup guide](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) walks you through setting up the features in Azure Active Directory Basic, like group-based access management, self-service password reset for cloud apps, and Azure Active Directory Application Proxy for publishing on-premises web apps.</span></span>


