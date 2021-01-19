---
title: Cấu hình và khắc phục sự cố tuyên bố SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7799"
- "9004356"
ms.openlocfilehash: 306d2f451856a66f06447e3acd73e065da71cd64
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901295"
---
# <a name="configure-and-troubleshoot-saml-claims"></a><span data-ttu-id="dbba2-102">Cấu hình và khắc phục sự cố tuyên bố SAML</span><span class="sxs-lookup"><span data-stu-id="dbba2-102">Configure and troubleshoot SAML claims</span></span>

<span data-ttu-id="dbba2-103">Để cấu hình và khắc phục sự cố tuyên bố SAML:</span><span class="sxs-lookup"><span data-stu-id="dbba2-103">To configure and troubleshoot SAML claims:</span></span>

1. <span data-ttu-id="dbba2-104">Làm theo các bước được nêu trong [bài viết này](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) để đặt cấu hình yêu cầu bồi thường vai trò được phát hành trong các ứng dụng trong hồ sơ hồ sơ SAML.</span><span class="sxs-lookup"><span data-stu-id="dbba2-104">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) to configure the role claim issued in the SAML token for enterprise applications.</span></span>
2. <span data-ttu-id="dbba2-105">Hãy làm theo các bước trong [bài viết này](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization) để tùy chỉnh tuyên bố đã phát hành trong các ứng dụng SAML token dành cho doanh nghiệp.</span><span class="sxs-lookup"><span data-stu-id="dbba2-105">Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization) to customize claims issued in the SAML token for enterprise applications.</span></span>
3. <span data-ttu-id="dbba2-106">Làm theo các bước trong [bài viết này](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) để tùy chỉnh tuyên bố phát ra bằng thẻ cho một ứng dụng cụ thể trong một đối tượng thuê.</span><span class="sxs-lookup"><span data-stu-id="dbba2-106">Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) to customize claims emitted in tokens for a specific app in a tenant.</span></span>
4. <span data-ttu-id="dbba2-107">Đọc [bài viết này](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) để hiểu cách làm việc với các ứng dụng nhận thức tuyên bố trong proxy Application.</span><span class="sxs-lookup"><span data-stu-id="dbba2-107">Read [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) to understand working with claims-aware apps in Application Proxy.</span></span>