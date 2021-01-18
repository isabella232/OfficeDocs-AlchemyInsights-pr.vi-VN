---
title: Đồng bộ hóa dịch vụ miền
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885774"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="76b11-102">Đồng bộ hóa dịch vụ miền</span><span class="sxs-lookup"><span data-stu-id="76b11-102">Domain service synchronization</span></span>

<span data-ttu-id="76b11-103">Đối tượng và thông tin đăng nhập trong tên miền được quản lý Dịch vụ Azure Active Directory (Azure AD DS) có thể được tạo cục bộ trong tên miền hoặc được đồng bộ hóa từ một đối tượng thuê Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="76b11-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="76b11-104">Khi bạn lần đầu tiên triển khai Azure AD DS, một đồng bộ hóa theo cách tự động được cấu hình và khởi tạo để sao chép các đối tượng từ Azure AD.</span><span class="sxs-lookup"><span data-stu-id="76b11-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="76b11-105">Đồng bộ một chiều này vẫn tiếp tục chạy trong nền để giữ cho tên miền Azure AD DS được quản lý với bất kỳ thay đổi nào từ Azure AD.</span><span class="sxs-lookup"><span data-stu-id="76b11-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="76b11-106">Không có đồng bộ hóa xuất hiện từ Azure AD DS trở lại Azure AD.</span><span class="sxs-lookup"><span data-stu-id="76b11-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="76b11-107">Để biết thêm chi tiết về việc đồng bộ hóa dịch vụ tên miền Azure Active Directory, hãy xem [Domain Dịch vụ đồng bộ](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span><span class="sxs-lookup"><span data-stu-id="76b11-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
