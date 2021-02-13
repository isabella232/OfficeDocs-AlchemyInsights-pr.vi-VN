---
title: Triển khai Microsoft Edge đến iOS, iPadOS và Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194582"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="15cf8-102">Triển khai Microsoft Edge đến iOS, iPadOS và Android</span><span class="sxs-lookup"><span data-stu-id="15cf8-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="15cf8-103">Kịch bản được hướng dẫn tóm tắt dưới đây sẽ giúp bạn gán Microsoft Edge cho người dùng iOS, iPadOS và thiết bị Android.</span><span class="sxs-lookup"><span data-stu-id="15cf8-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="15cf8-104">Nếu bạn bị chặn người dùng từ các thiết bị di động đăng ký, kịch bản hướng dẫn này sẽ không hoạt động và người dùng sẽ cần phải cài đặt Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="15cf8-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="15cf8-105">Kịch bản hướng dẫn liên quan đến các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="15cf8-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="15cf8-106">OLSync</span><span class="sxs-lookup"><span data-stu-id="15cf8-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="15cf8-107">Quen</span><span class="sxs-lookup"><span data-stu-id="15cf8-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="15cf8-108">Niệm</span><span class="sxs-lookup"><span data-stu-id="15cf8-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="15cf8-109">60A</span><span class="sxs-lookup"><span data-stu-id="15cf8-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="15cf8-110">Cu</span><span class="sxs-lookup"><span data-stu-id="15cf8-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="15cf8-111">Xem lại và tạo</span><span class="sxs-lookup"><span data-stu-id="15cf8-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="15cf8-112">Sau khi bạn hoàn thành các bước trong kịch bản hướng dẫn, chính sách của Microsoft InTune sẽ cho phép các tính năng sau đây của Microsoft Edge for Business:</span><span class="sxs-lookup"><span data-stu-id="15cf8-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="15cf8-113">Định danh kép</span><span class="sxs-lookup"><span data-stu-id="15cf8-113">Dual identity</span></span>
- <span data-ttu-id="15cf8-114">Tích hợp với chính sách bảo vệ ứng dụng Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="15cf8-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="15cf8-115">Tích hợp với ứng dụng Azure Active Directory proxy</span><span class="sxs-lookup"><span data-stu-id="15cf8-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="15cf8-116">Lối tắt trang chủ và mục yêu thích được quản lý</span><span class="sxs-lookup"><span data-stu-id="15cf8-116">Managed favorites and home page shortcuts</span></span>
