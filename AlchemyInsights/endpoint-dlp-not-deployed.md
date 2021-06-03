---
title: DLP điểm cuối không được triển khai đến thiết bị của người dùng
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731873"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="130c4-102">DLP điểm cuối không được triển khai đến thiết bị của người dùng</span><span class="sxs-lookup"><span data-stu-id="130c4-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="130c4-103">Nếu thiết đặt Ngăn mất dữ liệu điểm cuối (DLP) chưa được áp dụng cho thiết bị của người dùng, hãy xác nhận rằng bạn đáp ứng các yêu cầu sau:</span><span class="sxs-lookup"><span data-stu-id="130c4-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="130c4-104">Windows 10 bản x64 bản dựng 1809 trở lên đã được cài đặt trên thiết bị.</span><span class="sxs-lookup"><span data-stu-id="130c4-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="130c4-105">Đã cài đặt phiên bản máy khách chống phần mềm xấu phiên bản 4.18.2009.7 trở lên.</span><span class="sxs-lookup"><span data-stu-id="130c4-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="130c4-106">Thiết bị là một **trong những thiết** bị sau:</span><span class="sxs-lookup"><span data-stu-id="130c4-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="130c4-107">Azure Active Directory (Azure AD) đã tham gia</span><span class="sxs-lookup"><span data-stu-id="130c4-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="130c4-108">Đã kết hợp Azure AD</span><span class="sxs-lookup"><span data-stu-id="130c4-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="130c4-109">Đã đăng ký AAD</span><span class="sxs-lookup"><span data-stu-id="130c4-109">AAD registered</span></span>

- <span data-ttu-id="130c4-110">Để thực thi các hành động chính sách, hãy đảm bảo Chromium Microsoft Edge được cài đặt trên thiết bị điểm cuối.</span><span class="sxs-lookup"><span data-stu-id="130c4-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="130c4-111">Để biết thêm yêu cầu về việc triển khai DLP Điểm cuối, hãy [xem Bắt đầu với ngăn mất dữ liệu Điểm cuối](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span><span class="sxs-lookup"><span data-stu-id="130c4-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>