---
title: Cấu hình DLP điểm cuối
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/03/2020
ms.locfileid: "46556030"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="b70ff-102">Cấu hình DLP điểm cuối</span><span class="sxs-lookup"><span data-stu-id="b70ff-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="b70ff-103">Microsoft Endpoint DLP cho phép bạn mở rộng khả năng giám sát và bảo vệ DLP thông tin nhạy cảm trên các thiết bị Windows 10.</span><span class="sxs-lookup"><span data-stu-id="b70ff-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="b70ff-104">Sau khi thiết bị được onboarded vào quản lý thiết bị, bạn có thể tạo DLP chính sách để thực thi các hành động bảo vệ trên các mục.</span><span class="sxs-lookup"><span data-stu-id="b70ff-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="b70ff-105">Explorer hoạt động có thể được sử dụng để giám sát hoạt động cho các mục nhạy cảm.</span><span class="sxs-lookup"><span data-stu-id="b70ff-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="b70ff-106">Để biết thêm thông tin, xem [thiết bị Onboarding vào quản lý thiết bị](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="b70ff-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="b70ff-107">Để bắt đầu với DLP Endpoint:</span><span class="sxs-lookup"><span data-stu-id="b70ff-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="b70ff-108">Đảm bảo bạn có giấy phép SKU/đăng ký thích hợp.</span><span class="sxs-lookup"><span data-stu-id="b70ff-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="b70ff-109">Để biết thêm thông tin, xem [giấy phép SKU/đăng ký](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="b70ff-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="b70ff-110">Kiểm tra các quyền cần thiết để cho phép quản lý thiết bị, truy cập trang bộ nhớ ngoài hoặc bật/tắt giám sát thiết bị.</span><span class="sxs-lookup"><span data-stu-id="b70ff-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="b70ff-111">Để biết thêm thông tin, xem [quyền](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="b70ff-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="b70ff-112">Thiết bị trên máy vào quản lý thiết bị bằng thủ tục thiết bị bộ nhớ ngoài.</span><span class="sxs-lookup"><span data-stu-id="b70ff-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="b70ff-113">Nếu bạn đang thiếu tùy chọn thiết bị tích hợp (xem trước) trong M365 **cài đặt**tuân thủ, xác nhận bạn có giấy phép và quyền được tham chiếu ở trên.</span><span class="sxs-lookup"><span data-stu-id="b70ff-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="b70ff-114">Để biết thêm thông tin, xem [thiết bị Onboarding](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="b70ff-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="b70ff-115">Tạo chính sách DLP để bảo vệ các mục nhạy cảm của bạn.</span><span class="sxs-lookup"><span data-stu-id="b70ff-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="b70ff-116">Để biết thông tin, xem các [trường hợp chính sách DLP điểm cuối](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="b70ff-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="b70ff-117">Để biết thêm thông tin về Microsoft Endpoint DLP, [hãy xem Tìm hiểu về microsoft 365 điểm cuối dữ liệu mất mát (xem trước)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="b70ff-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>