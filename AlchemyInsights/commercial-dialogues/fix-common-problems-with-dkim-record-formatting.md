---
title: Khắc phục các sự cố phổ biến với định dạng bản ghi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750751"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="d8057-102">Khắc phục các sự cố phổ biến với định dạng bản ghi</span><span class="sxs-lookup"><span data-stu-id="d8057-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="d8057-103">Hầu hết các vấn đề về định danh trong thiết lập liên quan đến các bản ghi DNS không chính xác.</span><span class="sxs-lookup"><span data-stu-id="d8057-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="d8057-104">Để khắc phục các sự cố về thiết lập, hãy xác minh rằng bản ghi CNAME (**không phải** bản ghi TXT) được định dạng chính xác.</span><span class="sxs-lookup"><span data-stu-id="d8057-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="d8057-105">Để biết thêm thông tin, hãy xem [những điều bạn cần làm để thiết lập theo cách thủ công trong Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span><span class="sxs-lookup"><span data-stu-id="d8057-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="d8057-106">Nếu bạn cần trợ giúp với các bản ghi DNS nói chung, hãy xem [tạo bản ghi DNS tại bất kỳ nhà cung cấp lưu trữ DNS nào cho Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="d8057-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="d8057-107">Sau khi bạn tạo hoặc Cập Nhật bản ghi DNS của bạn tại dịch vụ lưu trữ DNS cho tên miền của bạn, bạn sẽ cần phải đợi cho bản ghi DNS để tuyên truyền.</span><span class="sxs-lookup"><span data-stu-id="d8057-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
