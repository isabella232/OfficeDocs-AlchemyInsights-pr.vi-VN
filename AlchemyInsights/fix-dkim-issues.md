---
title: Khắc phục sự cố thiết lập DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506796"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="834a6-102">Khắc phục sự cố thiết lập DKIM</span><span class="sxs-lookup"><span data-stu-id="834a6-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="834a6-103">Nếu bạn gặp sự cố cho phép DKIM cho miền tuỳ chỉnh của bạn, sử dụng các bước sau:</span><span class="sxs-lookup"><span data-stu-id="834a6-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="834a6-104">Hầu hết các sự cố thiết lập DKIM có liên quan đến bản ghi DNS không chính xác.</span><span class="sxs-lookup"><span data-stu-id="834a6-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="834a6-105">Kiểm tra bản ghi DKIM CNAME (**không** phải bản ghi TXT) được định dạng chính xác.</span><span class="sxs-lookup"><span data-stu-id="834a6-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="834a6-106">Để biết thêm thông tin, xem [chủ đề](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)này.</span><span class="sxs-lookup"><span data-stu-id="834a6-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="834a6-107">Sau khi bạn tạo hoặc Cập Nhật bản ghi DKIM DNS của mình tại dịch vụ lưu trữ DNS cho miền của bạn (thông thường, công ty đăng ký tên miền của bạn), hãy đợi bản ghi DNS truyền.</span><span class="sxs-lookup"><span data-stu-id="834a6-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="834a6-108">Nếu bạn không thể tạo bản ghi DKIM DNS trong Trung tâm quản trị, bạn có thể thay thế \<CustomDomain\> bằng miền tuỳ chỉnh của bạn (ví dụ: contoso.com) và chạy lệnh này trong [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="834a6-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
