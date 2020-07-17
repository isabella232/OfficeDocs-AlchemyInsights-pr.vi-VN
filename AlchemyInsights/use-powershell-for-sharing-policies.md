---
title: Sử dụng PowerShell để chia sẻ chính sách và mối quan hệ tổ chức
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862161"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="7cb65-102">Sử dụng PowerShell để chia sẻ chính sách và mối quan hệ tổ chức</span><span class="sxs-lookup"><span data-stu-id="7cb65-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="7cb65-103">Mối quan hệ tổ chức vui lòng đánh giá thông tin chi tiết cú pháp và tham số cho: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-organizationmối quan](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship)hệ, [thiết lập organizationmối quan](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) hệ và [loại bỏ organizationmối quan hệ](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="7cb65-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="7cb65-104">Để tạo chính sách chia sẻ sử dụng [mới SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="7cb65-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="7cb65-105">Để [áp dụng chính sách chia sẻ cho hộp thư hoặc người dùng](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) bạn cần sử dụng kết hợp [hộp thư thiết lập](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) và [nhận hộp thư](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) với chính sách mới được tạo ra.</span><span class="sxs-lookup"><span data-stu-id="7cb65-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="7cb65-106">Để [sửa đổi, vô hiệu hoá hoặc xoá một chính sách chia sẻ](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) bạn cần sử dụng [thiết lập sharingpolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) và [loại bỏ-sharingpolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="7cb65-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="7cb65-107">**Đối với sự hiểu biết đầy đủ của chủ đề này xin vui lòng đọc:**</span><span class="sxs-lookup"><span data-stu-id="7cb65-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="7cb65-108">Chia sẻ trong Exchange Online</span><span class="sxs-lookup"><span data-stu-id="7cb65-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)