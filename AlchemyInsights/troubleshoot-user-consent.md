---
title: Khắc phục sự cố người dùng
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901624"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="64b00-102">Khắc phục sự cố người dùng</span><span class="sxs-lookup"><span data-stu-id="64b00-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="64b00-103">Bạn có thể cấu hình cách thức người dùng cuối đồng ý với các ứng dụng thông qua Azure Portal hoặc PowerShell.</span><span class="sxs-lookup"><span data-stu-id="64b00-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="64b00-104">Xem [thiết đặt chấp thuận của người dùng](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="64b00-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="64b00-105">Người quản trị cũng có thể sử dụng [API của Microsoft graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) để cấp sự đồng ý cho phép ủy quyền thay mặt cho một người dùng duy nhất.</span><span class="sxs-lookup"><span data-stu-id="64b00-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="64b00-106">Để biết thêm thông tin, hãy xem [nhận quyền truy nhập thay mặt cho người dùng](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="64b00-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="64b00-107">[Lỗi người dùng chấp thuận](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): bài viết này thảo luận về các lỗi có thể xảy ra trong quá trình đồng ý với một ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="64b00-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="64b00-108">Nếu bạn đang khắc phục sự cố không mong đợi lời nhắc không chứa bất kỳ thông báo lỗi nào, hãy xem [kịch bản xác thực cho AZURE AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="64b00-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>