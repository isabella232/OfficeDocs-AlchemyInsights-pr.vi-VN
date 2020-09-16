---
title: Khắc phục sự cố về cài đặt trong thiết lập
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744972"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="37bf0-102">Khắc phục sự cố về cài đặt trong thiết lập</span><span class="sxs-lookup"><span data-stu-id="37bf0-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="37bf0-103">Nếu bạn gặp sự cố khi bật bkim cho tên miền riêng của mình, hãy thực hiện các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="37bf0-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="37bf0-104">Hầu hết các vấn đề về thiết lập được định nhất liên quan đến các bản ghi DNS không chính xác.</span><span class="sxs-lookup"><span data-stu-id="37bf0-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="37bf0-105">Xác minh bản ghi CNAME (**not** a txt Record) được định dạng chính xác.</span><span class="sxs-lookup"><span data-stu-id="37bf0-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="37bf0-106">Để biết thêm thông tin, hãy xem [chủ đề](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)này.</span><span class="sxs-lookup"><span data-stu-id="37bf0-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="37bf0-107">Sau khi bạn tạo hoặc Cập Nhật bản ghi DNS của bạn tại dịch vụ lưu trữ DNS cho tên miền của bạn (thường là cơ quan đăng ký tên miền của bạn), hãy chờ cho bản ghi DNS để tuyên truyền.</span><span class="sxs-lookup"><span data-stu-id="37bf0-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="37bf0-108">Nếu bạn không thể tạo bản ghi DNS của YKIM trong Trung tâm quản trị, bạn có thể thay thế \<CustomDomain\> bằng tên miền riêng của bạn (ví dụ, contoso.com) và chạy lệnh này trong [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="37bf0-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
