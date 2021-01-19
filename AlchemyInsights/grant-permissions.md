---
title: Cấp quyền
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
- "7784"
ms.openlocfilehash: 9e686bd33414512b0a3a2bc24477832a508537a8
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901621"
---
# <a name="grant-permissions"></a><span data-ttu-id="2072c-102">Cấp quyền</span><span class="sxs-lookup"><span data-stu-id="2072c-102">Grant permissions</span></span>

1. <span data-ttu-id="2072c-103">Cấp sự **đồng ý của người quản trị** đối tượng thuê: xem cấp phép người quản trị toàn bộ đối tượng thuê cho [một ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) cho các hướng dẫn từng bước để cấp sự đồng ý người quản trị đối tượng thuê từ Azure Portal, bằng cách sử dụng Azure AD PowerShell hoặc từ đồng ý lời nhắc chính nó.</span><span class="sxs-lookup"><span data-stu-id="2072c-103">**Granting tenant-wide admin consent**: See [Grant tenant-wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for step-by-step instructions for granting tenant-wide admin consent from the Azure portal, using Azure AD PowerShell, or from the consent prompt itself.</span></span>
1. <span data-ttu-id="2072c-104">Cấp phép **chấp thuận thay mặt cho một người dùng cụ thể**: thay vì cấp sự đồng ý cho toàn bộ tổ chức, người quản trị cũng có thể sử dụng [API của Microsoft graph](https://docs.microsoft.com/graph/use-the-api) để cấp sự đồng ý cho phép ủy quyền thay mặt cho một người dùng duy nhất.</span><span class="sxs-lookup"><span data-stu-id="2072c-104">**Granting consent on behalf of a specific user**: Instead of granting consent for the entire organization, an administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="2072c-105">Để biết thêm thông tin, hãy xem [nhận quyền truy nhập thay mặt cho người dùng](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="2072c-105">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>