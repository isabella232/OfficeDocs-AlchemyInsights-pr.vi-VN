---
title: Chính sách bảo vệ ứng dụng
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 929400dcf0ca18ce8f52cb11e5c907064449480e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716915"
---
# <a name="application-protection-policy"></a><span data-ttu-id="1d862-102">Chính sách bảo vệ ứng dụng</span><span class="sxs-lookup"><span data-stu-id="1d862-102">Application protection policy</span></span>

<span data-ttu-id="1d862-103">Nếu bạn mới dùng chính sách bảo vệ ứng dụng (ứng dụng), hãy xem [tổng quan về chính sách bảo vệ ứng dụng](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="1d862-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="1d862-104">Để bắt đầu sử dụng ứng dụng, hãy xem [cách tạo và gán các chính sách bảo vệ ứng dụng](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="1d862-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="1d862-105">Các yêu cầu về chính sách bảo vệ ứng dụng:</span><span class="sxs-lookup"><span data-stu-id="1d862-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="1d862-106">Người dùng có giấy phép InTune hoặc EMS.</span><span class="sxs-lookup"><span data-stu-id="1d862-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="1d862-107">Người dùng thuộc các chính sách bảo vệ ứng dụng được mục tiêu theo nhóm.</span><span class="sxs-lookup"><span data-stu-id="1d862-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="1d862-108">Chỉ có một người dùng công ty được đăng nhập vào các ứng dụng được bảo vệ trên thiết bị.</span><span class="sxs-lookup"><span data-stu-id="1d862-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="1d862-109">Ứng dụng này đã triển khai [SDK InTune](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="1d862-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="1d862-110">Để có danh sách các ứng dụng hỗ trợ SDK, hãy xem các [ứng dụng đã được bảo vệ của Microsoft InTune](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="1d862-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="1d862-111">Các chính sách áp dụng sau khi một người dùng đáp ứng các dấu hiệu nêu trên vào ứng dụng được kích hoạt trong một bộ điều chỉnh SDK.</span><span class="sxs-lookup"><span data-stu-id="1d862-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="1d862-112">Cách dễ nhất để xác định xem một chính sách được áp dụng là bằng yêu cầu người dùng đã thiết lập mã pin trong chính sách.</span><span class="sxs-lookup"><span data-stu-id="1d862-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="1d862-113">Để biết thêm thông tin, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="1d862-113">For more information, see:</span></span>

[<span data-ttu-id="1d862-114">Khắc phục sự cố câu hỏi thường gặp về ứng dụng</span><span class="sxs-lookup"><span data-stu-id="1d862-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="1d862-115">Cách xác thực thiết lập chính sách bảo vệ ứng dụng của bạn</span><span class="sxs-lookup"><span data-stu-id="1d862-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="1d862-116">Tìm hiểu thời gian chuyển phát của chính sách bảo vệ ứng dụng</span><span class="sxs-lookup"><span data-stu-id="1d862-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="1d862-117">Cách giám sát các chính sách bảo vệ ứng dụng</span><span class="sxs-lookup"><span data-stu-id="1d862-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)