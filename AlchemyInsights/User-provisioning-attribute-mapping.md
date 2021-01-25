---
title: Ánh xạ thuộc tính cung cấp người dùng
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949901"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="5d988-102">Ánh xạ thuộc tính cung cấp người dùng</span><span class="sxs-lookup"><span data-stu-id="5d988-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="5d988-103">Để khắc phục sự cố đã biết về bản đồ thuộc tính, hãy xem [ánh xạ thuộc tính](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="5d988-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="5d988-104">Microsoft Azure Active Directory (AD) cung cấp hỗ trợ cho người dùng cung cấp cho các ứng dụng SaaS bên thứ ba, chẳng hạn như Salesforce, G Suite và những người khác.</span><span class="sxs-lookup"><span data-stu-id="5d988-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="5d988-105">Nếu bạn cho phép người dùng cung cấp cho ứng dụng SaaS của bên thứ ba, cổng thông tin Azure điều khiển các giá trị thuộc tính của nó thông qua các thuộc tính-ánh xạ.</span><span class="sxs-lookup"><span data-stu-id="5d988-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="5d988-106">Để tìm hiểu cách tùy chỉnh thuộc tính mặc định-ánh xạ, hãy xem [tùy chỉnh thuộc tính cung cấp người dùng-ánh xạ cho các ứng dụng Saas trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="5d988-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="5d988-107">Để tìm hiểu thêm về cung cấp người dùng ứng dụng SaaS, hãy xem mục [cung cấp người dùng Saas tự động ứng dụng trong AZURE AD là gì?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="5d988-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="5d988-108">Khi tùy chỉnh thuộc tính-ánh xạ đối với người dùng cung cấp, bạn có thể thấy rằng thuộc tính mà bạn muốn ánh xạ không xuất hiện trong danh sách thuộc tính nguồn.</span><span class="sxs-lookup"><span data-stu-id="5d988-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="5d988-109">[Đồng bộ thuộc tính từ Active Directory tại chỗ của bạn với AZURE AD để cung](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) cấp cho một bài viết ứng dụng cho bạn biết cách thêm thuộc tính bị thiếu bằng cách đồng bộ hóa từ quảng cáo tại cơ sở của bạn thành Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5d988-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
