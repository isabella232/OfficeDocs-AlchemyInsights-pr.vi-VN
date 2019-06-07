---
title: Khắc phục vấn đề thiết lập DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765549"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="98f30-102">Khắc phục vấn đề thiết lập DKIM</span><span class="sxs-lookup"><span data-stu-id="98f30-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="98f30-103">Nếu bạn gặp vấn đề cho phép DKIM cho miền tuỳ chỉnh của bạn, sử dụng các bước sau:</span><span class="sxs-lookup"><span data-stu-id="98f30-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="98f30-104">Hầu hết các vấn đề thiết lập DKIM có liên quan đến bản ghi DNS không chính xác.</span><span class="sxs-lookup"><span data-stu-id="98f30-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="98f30-105">Xác minh DKIM bản ghi CNAME (**không phải** bản ghi TXT) được định dạng đúng.</span><span class="sxs-lookup"><span data-stu-id="98f30-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="98f30-106">Để biết thêm chi tiết, xem [chủ đề](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)này.</span><span class="sxs-lookup"><span data-stu-id="98f30-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="98f30-107">Sau khi bạn tạo hoặc Cập Nhật bản ghi DKIM DNS tại DNS hosting dịch vụ cho tên miền của bạn (thông thường, tên miền đăng ký của bạn), chờ đợi cho các bản ghi DNS để tuyên truyền.</span><span class="sxs-lookup"><span data-stu-id="98f30-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="98f30-108">Nếu bạn không thể tạo DKIM DNS hồ sơ tại Trung tâm quản trị, bạn có thể thay thế \<CustomDomain\> với tên miền riêng của bạn (ví dụ: contoso.com) và chạy lệnh này trong [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="98f30-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
