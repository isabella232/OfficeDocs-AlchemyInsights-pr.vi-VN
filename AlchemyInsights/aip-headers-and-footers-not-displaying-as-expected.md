---
title: 'AIP: đầu trang và chân trang không hiển thị như mong đợi'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4541"
ms.openlocfilehash: 5f50fc1d38618017bca61b4e9290d9893983534e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821721"
---
# <a name="aip-headers-and-footers-not-displaying-as-expected"></a><span data-ttu-id="16165-102">AIP: đầu trang và chân trang không hiển thị như mong đợi</span><span class="sxs-lookup"><span data-stu-id="16165-102">AIP: Headers and footers not displaying as expected</span></span>

<span data-ttu-id="16165-103">Nếu bạn đang gặp sự cố với dấu hiệu trực quan không hiển thị như mong muốn, hãy xem các hướng dẫn sau đây:</span><span class="sxs-lookup"><span data-stu-id="16165-103">If you are experiencing issues with visual markings not displaying as expected, view the following guidelines:</span></span>

1. <span data-ttu-id="16165-104">Hãy đảm bảo bạn đã xem lại [khi có dấu hiệu trực quan được áp dụng](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="16165-104">Make sure you have reviewed [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="16165-105">Đối với ghi nhãn Office, hãy xem lại [khi Office 365 áp dụng đánh dấu nội dung và mã hóa](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption).</span><span class="sxs-lookup"><span data-stu-id="16165-105">For Office labeling, review [When Office 365 applies content marking and encryption](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption).</span></span>
3. <span data-ttu-id="16165-106">Nếu bạn muốn loại bỏ đầu trang/chân trang hiện có, hãy xem lại [loại bỏ đầu trang và chân trang khỏi các giải pháp ghi nhãn khác](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions).</span><span class="sxs-lookup"><span data-stu-id="16165-106">If you want to remove existing headers/footers, review [Remove headers and footers from other labeling solutions](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions).</span></span>

<span data-ttu-id="16165-107">Nếu bạn vẫn gặp sự cố này, hãy thu thập Nhật ký máy khách bảo vệ thông tin Azure và đính kèm các Nhật ký đã xuất vào vé này.</span><span class="sxs-lookup"><span data-stu-id="16165-107">If you are still experiencing the issue, collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

<span data-ttu-id="16165-108">**Xuất Nhật ký bảo vệ thông tin Azure**</span><span class="sxs-lookup"><span data-stu-id="16165-108">**Export Azure Information Protection logs**</span></span>

1. <span data-ttu-id="16165-109">Mở tài liệu Office hoặc tạo email mới trong Outlook.</span><span class="sxs-lookup"><span data-stu-id="16165-109">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="16165-110">Bấm vào **bảo vệ/**  >  **Trợ giúp và phản hồi** nhạy cảm.</span><span class="sxs-lookup"><span data-stu-id="16165-110">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="16165-111">Bấm **xuất Nhật ký**.</span><span class="sxs-lookup"><span data-stu-id="16165-111">Click **Export Logs**.</span></span>
4. <span data-ttu-id="16165-112">Lưu Nhật ký vào lựa chọn vị trí của bạn và đính kèm chúng vào yêu cầu dịch vụ này.</span><span class="sxs-lookup"><span data-stu-id="16165-112">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="16165-113">Để biết thêm thông tin, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="16165-113">For additional information, see:</span></span>

- [<span data-ttu-id="16165-114">Cách đặt cấu hình nhãn cho các dấu hiệu trực quan cho bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="16165-114">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="16165-115">Xem lại tài liệu bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="16165-115">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="16165-116">Các yêu cầu về bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="16165-116">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="16165-117">Hướng dẫn nhanh về bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="16165-117">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="16165-118">Tải xuống máy khách bảo vệ thông tin về Azure</span><span class="sxs-lookup"><span data-stu-id="16165-118">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
