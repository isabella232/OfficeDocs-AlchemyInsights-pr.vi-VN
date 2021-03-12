---
title: Sử dụng PowerShell để chia sẻ chính sách và mối quan hệ tổ chức
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709488"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="5336c-102">Sử dụng PowerShell để chia sẻ chính sách và mối quan hệ tổ chức</span><span class="sxs-lookup"><span data-stu-id="5336c-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="5336c-103">Đối với các mối quan hệ tổ chức, vui lòng xem lại thông tin chi tiết về cú pháp và tham số cho: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-organizationmối](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship)quan hệ, [Set-organizationmối](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  quan hệ và  [loại bỏ](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="5336c-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="5336c-104">Để tạo chính sách chia sẻ sử dụng [mới-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="5336c-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="5336c-105">Để  [áp dụng chính sách chia sẻ cho một hộp thư hoặc người dùng](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  mà bạn cần sử dụng kết hợp  [hộp thư đặt](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) và [nhận hộp thư](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) với chính sách mới được tạo.</span><span class="sxs-lookup"><span data-stu-id="5336c-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="5336c-106">Để  [sửa đổi, tắt hoặc loại bỏ chính sách chia sẻ,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  bạn cần sử dụng  [thiết đặt](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) chính sách và [loại bỏ](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="5336c-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="5336c-107">**Để biết đầy đủ về chủ đề này, vui lòng đọc:**</span><span class="sxs-lookup"><span data-stu-id="5336c-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="5336c-108">Chia sẻ trong Exchange Online</span><span class="sxs-lookup"><span data-stu-id="5336c-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)