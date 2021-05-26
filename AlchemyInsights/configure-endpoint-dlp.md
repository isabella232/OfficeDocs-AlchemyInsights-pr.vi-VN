---
title: Đặt cấu hình DLP Điểm cuối
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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657951"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="88130-102">Đặt cấu hình DLP Điểm cuối</span><span class="sxs-lookup"><span data-stu-id="88130-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="88130-103">DLP Điểm cuối của Microsoft cho phép bạn mở rộng khả năng bảo vệ và theo dõi DLP đối với thông tin nhạy cảm Windows 10 thiết bị.</span><span class="sxs-lookup"><span data-stu-id="88130-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="88130-104">Sau khi thiết bị được triển lý vào quản lý thiết bị, bạn có thể tạo các chính sách DLP để thực thi các hành động bảo vệ trên các mục.</span><span class="sxs-lookup"><span data-stu-id="88130-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="88130-105">Có thể dùng Activity Explorer để giám sát hoạt động cho các mục nhạy cảm.</span><span class="sxs-lookup"><span data-stu-id="88130-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="88130-106">Để biết thêm thông tin, hãy xem [Mục Các thiết bị tích hợp vào quản lý thiết bị](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="88130-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="88130-107">Để bắt đầu với DLP Điểm cuối:</span><span class="sxs-lookup"><span data-stu-id="88130-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="88130-108">Ensure you have the appropriate SKU/subscriptions licensing.</span><span class="sxs-lookup"><span data-stu-id="88130-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="88130-109">Để biết thêm thông tin, hãy [xem mục Cấp phép SKU/đăng ký.](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)</span><span class="sxs-lookup"><span data-stu-id="88130-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="88130-110">Kiểm tra các quyền cần thiết để cho phép quản lý thiết bị, truy nhập trang trình phát hoặc bật/tắt chức năng giám sát thiết bị.</span><span class="sxs-lookup"><span data-stu-id="88130-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="88130-111">Để biết thêm thông tin, hãy [xem Quyền](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="88130-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="88130-112">Đưa thiết bị vào Quản lý thiết bị bằng cách làm theo quy trình trên thiết bị.</span><span class="sxs-lookup"><span data-stu-id="88130-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="88130-113">Để biết thêm thông tin, hãy [xem Mục Các thiết bị đang phát hành](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="88130-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="88130-114">Tạo chính sách DLP để bảo vệ các mục nhạy cảm của bạn.</span><span class="sxs-lookup"><span data-stu-id="88130-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="88130-115">Để biết thông tin, hãy [xem Các kịch bản chính sách DLP điểm cuối.](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)</span><span class="sxs-lookup"><span data-stu-id="88130-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="88130-116">Để biết thêm thông tin về DLP Điểm cuối Microsoft, hãy xem Tìm hiểu về cách Microsoft 365 ngăn mất dữ liệu điểm cuối [(bản xem trước).](/microsoft-365/compliance/endpoint-dlp-learn-about)</span><span class="sxs-lookup"><span data-stu-id="88130-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="88130-117">**Các bước Thu thập Dữ liệu Quan trọng nếu cần Hỗ trợ:**</span><span class="sxs-lookup"><span data-stu-id="88130-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="88130-118">Tải xuống [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="88130-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="88130-119">Chạy công cụ với tư cách là Người quản trị từ cửa sổ cmd:</span><span class="sxs-lookup"><span data-stu-id="88130-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="88130-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="88130-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="88130-121">Khi được nhắc nhập số phút để thu thập dấu **vết:**, hãy nhập số phút cần thiết để chạy kịch bản.</span><span class="sxs-lookup"><span data-stu-id="88130-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="88130-122">Chạy kịch bản.</span><span class="sxs-lookup"><span data-stu-id="88130-122">Run the scenario.</span></span>

<span data-ttu-id="88130-123">Thu thập đầu ra tệp Zip để tặng cho nhân viên Hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="88130-123">Collect the Zip file output to give to the Support agent.</span></span>
