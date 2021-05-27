---
title: Các chỉ báo không hoạt động khi sử dụng trình duyệt Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676577"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="5bf8c-102">Các chỉ báo không hoạt động khi sử dụng trình duyệt Edge</span><span class="sxs-lookup"><span data-stu-id="5bf8c-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="5bf8c-103">Sau khi bạn đã tạo Chỉ báo, Edge (Màn hình thông minh) không có chức năng này.</span><span class="sxs-lookup"><span data-stu-id="5bf8c-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="5bf8c-104">Để biết thêm thông tin, [hãy xem Tạo chỉ báo cho CÁC URL và URL/miền.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="5bf8c-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="5bf8c-105">Bước 1: Đảm bảo các bước sau</span><span class="sxs-lookup"><span data-stu-id="5bf8c-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="5bf8c-106">Xác minh rằng chỉ báo là chính xác (không có lỗi đánh máy trong IP/URL, sửa hành động, nhóm RBAC chính xác).</span><span class="sxs-lookup"><span data-stu-id="5bf8c-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="5bf8c-107">Hãy chờ tối thiểu 2 giờ sau khi tạo chỉ báo để tính đến độ trễ có thể xảy ra.</span><span class="sxs-lookup"><span data-stu-id="5bf8c-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="5bf8c-108">Xác nhận rằng (các) hệ thống được tích hợp vào Bộ bảo vệ Microsoft dành cho Điểm cuối.</span><span class="sxs-lookup"><span data-stu-id="5bf8c-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="5bf8c-109">Xác minh (các) hệ thống có thể liên lạc với Đám mây.</span><span class="sxs-lookup"><span data-stu-id="5bf8c-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="5bf8c-110">Xác minh rằng Smartscreen đã được bật và có thể tiếp cận bằng cách đi tới [site thử nghiệm](https://demo.smartscreen.msft.net).</span><span class="sxs-lookup"><span data-stu-id="5bf8c-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="5bf8c-111">Bước 2: Khắc phục sự cố tiềm ẩn</span><span class="sxs-lookup"><span data-stu-id="5bf8c-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="5bf8c-112">Hãy đảm bảo máy khách đáp ứng các yêu cầu.</span><span class="sxs-lookup"><span data-stu-id="5bf8c-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="5bf8c-113">Để biết chi tiết, [hãy xem Tạo chỉ báo cho CÁC URL và URL/tên miền](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="5bf8c-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="5bf8c-114">Đảm bảo rằng bạn đang chạy phiên bản trình duyệt Edge mới nhất.</span><span class="sxs-lookup"><span data-stu-id="5bf8c-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="5bf8c-115">Để tìm hiểu phiên bản mới nhất, [hãy xem Tìm hiểu xem bạn có phiên bản Microsoft Edge nào.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)</span><span class="sxs-lookup"><span data-stu-id="5bf8c-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="5bf8c-116">Khởi động lại trình duyệt Edge.</span><span class="sxs-lookup"><span data-stu-id="5bf8c-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="5bf8c-117">Dẫn hướng đến site mà bạn đã thiết lập một chỉ báo.</span><span class="sxs-lookup"><span data-stu-id="5bf8c-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="5bf8c-118">Nếu site không xuất hiện như mong đợi, hãy tiếp tục đến Bước 3.</span><span class="sxs-lookup"><span data-stu-id="5bf8c-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="5bf8c-119">Bước 3: Thu thập dữ liệu</span><span class="sxs-lookup"><span data-stu-id="5bf8c-119">Step 3: Collect data</span></span>

- <span data-ttu-id="5bf8c-120">Thu **thập dữ liệu chẩn đoán MDEClientAnalyzer.**</span><span class="sxs-lookup"><span data-stu-id="5bf8c-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="5bf8c-121">Để biết hướng dẫn, hãy [xem mục Các sự cố với máy tiếp thị đối với Microsoft Defender dành cho Điểm cuối.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="5bf8c-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="5bf8c-122">Nếu bạn cảm thấy thoải mái khi cài đặt và thu thập dấu vết Fiddler, hãy xem [Telerik Fiddler.](http://www.telerik.com/fiddler)</span><span class="sxs-lookup"><span data-stu-id="5bf8c-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="5bf8c-123">Nếu bạn muốn xem hướng dẫn từ Bộ hỗ trợ của Microsoft, hãy chọn biểu tượng Hỗ trợ bên dưới để mở trường hợp hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="5bf8c-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
