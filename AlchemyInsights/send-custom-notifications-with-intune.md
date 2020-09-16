---
title: Gửi thông báo tùy chỉnh bằng InTune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720668"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="da1e6-102">Cách gửi thông báo tùy chỉnh cho người dùng các thiết bị quản lý iOS và Android</span><span class="sxs-lookup"><span data-stu-id="da1e6-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="da1e6-103">Thông báo tùy chỉnh cho InTune được xử lý bởi ứng dụng cổng thông tin công ty trên thiết bị của người dùng.</span><span class="sxs-lookup"><span data-stu-id="da1e6-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="da1e6-104">Ứng dụng sau đó sẽ tạo ra thông báo đẩy trên thiết bị đó.</span><span class="sxs-lookup"><span data-stu-id="da1e6-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="da1e6-105">Sau đây là các điều kiện tiên quyết của thiết bị để hỗ trợ nhận thông báo tùy chỉnh và đối với ứng dụng để tạo thông báo đẩy:</span><span class="sxs-lookup"><span data-stu-id="da1e6-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="da1e6-106">Thiết bị phải có cài đặt ứng dụng cổng thông tin công ty.</span><span class="sxs-lookup"><span data-stu-id="da1e6-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="da1e6-107">Thiết bị phải cho phép ứng dụng cổng thông tin công ty gửi thông báo đẩy.</span><span class="sxs-lookup"><span data-stu-id="da1e6-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="da1e6-108">Khi ứng dụng được cài đặt hoặc Cập Nhật, nó sẽ nhắc người dùng để cho phép thông báo.</span><span class="sxs-lookup"><span data-stu-id="da1e6-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="da1e6-109">Thiết bị Android phải có cài đặt Google Play Services.</span><span class="sxs-lookup"><span data-stu-id="da1e6-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="da1e6-110">Thiết bị phải được đăng ký bằng InTune.</span><span class="sxs-lookup"><span data-stu-id="da1e6-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="da1e6-111">Để biết thêm thông tin, bao gồm cách gửi thư, hãy xem [tài liệu hướng dẫn tính năng](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="da1e6-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
