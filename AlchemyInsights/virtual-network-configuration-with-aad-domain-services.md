---
title: Cấu hình ảo với dịch vụ tên miền của Bad
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885781"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="2cf61-102">Cấu hình ảo với dịch vụ tên miền của Bad</span><span class="sxs-lookup"><span data-stu-id="2cf61-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="2cf61-103">Cấu hình ảo với dịch vụ tên miền của Bad liên quan đến các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="2cf61-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="2cf61-104">Kiểm tra trạng thái tên miền của bạn trên cổng thông tin Azure https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="2cf61-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="2cf61-105">Kiểm tra NSG của bạn để xem các quy tắc chặn cổng cần thiết để đồng bộ hóa trong dịch vụ tên miền Azure AD trên cổng thông tin https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="2cf61-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="2cf61-106">Đảm bảo rằng mạng ảo của bạn được triển khai trong cùng một vùng Azure với tên miền Azure AD Domain Services của bạn.</span><span class="sxs-lookup"><span data-stu-id="2cf61-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="2cf61-107">Đảm bảo bạn không có tên miền nào có cùng tên miền sẵn dùng trên mạng ảo.</span><span class="sxs-lookup"><span data-stu-id="2cf61-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="2cf61-108">Để biết thêm chi tiết về việc xem xét thiết kế trên Azure Virtual Network để hỗ trợ dịch vụ tên miền của Bad, hãy xem [xem xét mạng ảo](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="2cf61-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

