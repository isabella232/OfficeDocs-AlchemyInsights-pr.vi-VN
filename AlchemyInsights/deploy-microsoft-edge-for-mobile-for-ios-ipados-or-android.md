---
title: Triển khai Microsoft Edge cho điện thoại di động cho iOS/iPadOS hoặc Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003919"
- "6974"
ms.openlocfilehash: 98ab637b6ca0f2b3cfa98ae897d6ed1d9f36c3cd
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679949"
---
# <a name="deploy-microsoft-edge-for-mobile-for-iosipados-or-android"></a><span data-ttu-id="7a7a7-102">Triển khai Microsoft Edge cho điện thoại di động cho iOS/iPadOS hoặc Android</span><span class="sxs-lookup"><span data-stu-id="7a7a7-102">Deploy Microsoft Edge for Mobile for iOS/iPadOS or Android</span></span>

<span data-ttu-id="7a7a7-103">Kịch bản được hướng dẫn tóm tắt dưới đây sẽ giúp bạn gán Microsoft Edge cho người dùng iOS, iPadOS và thiết bị Android.</span><span class="sxs-lookup"><span data-stu-id="7a7a7-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span> <span data-ttu-id="7a7a7-104">Sau khi bạn hoàn thành các bước này, chính sách của Microsoft InTune sẽ cho phép các tính năng sau đây của Microsoft Edge for Business:</span><span class="sxs-lookup"><span data-stu-id="7a7a7-104">After you complete these steps, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="7a7a7-105">Định danh kép</span><span class="sxs-lookup"><span data-stu-id="7a7a7-105">Dual identity</span></span>
- <span data-ttu-id="7a7a7-106">Tích hợp với chính sách bảo vệ ứng dụng Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="7a7a7-106">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="7a7a7-107">Tích hợp với ứng dụng Azure Active Directory proxy</span><span class="sxs-lookup"><span data-stu-id="7a7a7-107">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="7a7a7-108">Lối tắt trang chủ và mục yêu thích được quản lý</span><span class="sxs-lookup"><span data-stu-id="7a7a7-108">Managed favorites and home page shortcuts</span></span>

> [!NOTE]
> <span data-ttu-id="7a7a7-109">Nếu bạn chặn người dùng từ các thiết bị di động đăng ký, kịch bản hướng dẫn này sẽ không hoạt động và người dùng sẽ cần phải cài đặt Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="7a7a7-109">If you blocked users from enrolling mobile devices, this guided scenario will not work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="7a7a7-110">Để triển khai Microsoft Edge cho điện thoại di động cho iOS/iPadOS hoặc Android, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="7a7a7-110">To deploy Microsoft Edge for Mobile for iOS/iPadOS or Android, see:</span></span>

1. [<span data-ttu-id="7a7a7-111">OLSync</span><span class="sxs-lookup"><span data-stu-id="7a7a7-111">Prerequisites</span></span>](https://go.microsoft.com/fwlink/?linkid=2133027)
2. [<span data-ttu-id="7a7a7-112">Quen</span><span class="sxs-lookup"><span data-stu-id="7a7a7-112">Introduction</span></span>](https://go.microsoft.com/fwlink/?linkid=2133520)
3. [<span data-ttu-id="7a7a7-113">Niệm</span><span class="sxs-lookup"><span data-stu-id="7a7a7-113">Basics</span></span>](https://go.microsoft.com/fwlink/?linkid=2133421)
4. [<span data-ttu-id="7a7a7-114">60A</span><span class="sxs-lookup"><span data-stu-id="7a7a7-114">Configuration</span></span>](https://go.microsoft.com/fwlink/?linkid=2133521)
5. [<span data-ttu-id="7a7a7-115">Cu</span><span class="sxs-lookup"><span data-stu-id="7a7a7-115">Assignments</span></span>](https://go.microsoft.com/fwlink/?linkid=2132869)
6. [<span data-ttu-id="7a7a7-116">Xem lại và tạo</span><span class="sxs-lookup"><span data-stu-id="7a7a7-116">Review and creation</span></span>](https://go.microsoft.com/fwlink/?linkid=2133522)
