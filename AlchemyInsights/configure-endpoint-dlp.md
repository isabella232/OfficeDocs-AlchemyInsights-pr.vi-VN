---
title: Cấu hình điểm cuối
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 406bc40fbe8a6306a2f74506ef1daf70b37283d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812137"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="9fcb1-102">Cấu hình điểm cuối</span><span class="sxs-lookup"><span data-stu-id="9fcb1-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="9fcb1-103">Microsoft điểm cuối cho phép bạn mở rộng khả năng bảo vệ và giám sát cho các thông tin nhạy cảm trên các thiết bị chạy Windows 10.</span><span class="sxs-lookup"><span data-stu-id="9fcb1-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="9fcb1-104">Sau khi thiết bị được onchéo vào quản lý thiết bị, bạn có thể tạo chính sách có quy định thực thi hành động bảo vệ trên các mục.</span><span class="sxs-lookup"><span data-stu-id="9fcb1-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="9fcb1-105">Có thể sử dụng trình khám phá hoạt động để theo dõi hoạt động cho các mục nhạy cảm.</span><span class="sxs-lookup"><span data-stu-id="9fcb1-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="9fcb1-106">Để biết thêm thông tin, hãy xem [thiết bị Onboarding vào quản lý thiết bị](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="9fcb1-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="9fcb1-107">Để bắt đầu với điểm cuối:</span><span class="sxs-lookup"><span data-stu-id="9fcb1-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="9fcb1-108">Đảm bảo bạn có các mã bản quyền/gói đăng ký phù hợp.</span><span class="sxs-lookup"><span data-stu-id="9fcb1-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="9fcb1-109">Để biết thêm thông tin, hãy xem [Mã sản phẩm/gói đăng ký](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="9fcb1-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="9fcb1-110">Kiểm tra các quyền cần thiết để cho phép quản lý thiết bị, truy nhập trang triển khai hoặc bật/tắt giám sát thiết bị.</span><span class="sxs-lookup"><span data-stu-id="9fcb1-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="9fcb1-111">Để biết thêm thông tin, hãy xem [quyền](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="9fcb1-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="9fcb1-112">Thiết bị onboard vào quản lý thiết bị bằng cách làm theo quy trình thiết bị triển khai.</span><span class="sxs-lookup"><span data-stu-id="9fcb1-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="9fcb1-113">Nếu bạn bị thiếu tùy chọn cài đặt Onboarding (bản xem trước) bên dưới  **thiết đặt**tuân thủ M365, hãy xác nhận bạn có giấy phép và quyền thích hợp được tham chiếu ở trên.</span><span class="sxs-lookup"><span data-stu-id="9fcb1-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="9fcb1-114">Để biết thêm thông tin, hãy xem [thiết bị Onboarding](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="9fcb1-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="9fcb1-115">Tạo chính sách có thể bảo vệ các mục nhạy cảm của bạn.</span><span class="sxs-lookup"><span data-stu-id="9fcb1-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="9fcb1-116">Để biết thông tin, hãy xem các [kịch bản chính sách điểm cuối](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="9fcb1-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="9fcb1-117">Để biết thêm thông tin về Microsoft điểm cuối, hãy xem [Tìm hiểu về ngăn chặn mất dữ liệu về microsoft 365 Endpoint (bản xem trước)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="9fcb1-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>