---
title: Gửi thông báo tùy chỉnh với InTune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886879"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="44a2d-102">Cách gửi thông báo tùy chỉnh cho người dùng thiết bị iOS và Android được quản lý</span><span class="sxs-lookup"><span data-stu-id="44a2d-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="44a2d-103">Thông báo tùy chỉnh dành cho InTune được xử lý bởi ứng dụng cổng thông tin công ty trên thiết bị của người dùng.</span><span class="sxs-lookup"><span data-stu-id="44a2d-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="44a2d-104">Ứng dụng sau đó tạo thông báo đẩy trên thiết bị đó.</span><span class="sxs-lookup"><span data-stu-id="44a2d-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="44a2d-105">Sau đây là điều kiện tiên quyết của thiết bị để hỗ trợ nhận thông báo tùy chỉnh và cho ứng dụng sau đó tạo thông báo đẩy:</span><span class="sxs-lookup"><span data-stu-id="44a2d-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="44a2d-106">Thiết bị phải cài đặt ứng dụng cổng thông tin công ty.</span><span class="sxs-lookup"><span data-stu-id="44a2d-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="44a2d-107">Thiết bị phải cho phép ứng dụng cổng thông tin công ty gửi thông báo đẩy.</span><span class="sxs-lookup"><span data-stu-id="44a2d-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="44a2d-108">Khi ứng dụng được cài đặt hoặc Cập Nhật, nó sẽ nhắc người dùng cho phép thông báo.</span><span class="sxs-lookup"><span data-stu-id="44a2d-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="44a2d-109">Thiết bị Android phải được cài đặt Google Play Services.</span><span class="sxs-lookup"><span data-stu-id="44a2d-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="44a2d-110">Thiết bị phải được đăng ký với InTune.</span><span class="sxs-lookup"><span data-stu-id="44a2d-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="44a2d-111">Để biết thêm thông tin, bao gồm cách gửi tin nhắn, hãy xem [tài liệu tính năng](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="44a2d-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
