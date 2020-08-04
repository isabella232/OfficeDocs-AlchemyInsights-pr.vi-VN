---
title: Sử dụng hồ sơ email với InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555756"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="491a2-102">Sử dụng hồ sơ email với InTune</span><span class="sxs-lookup"><span data-stu-id="491a2-102">Using email profiles with Intune</span></span>

<span data-ttu-id="491a2-103">InTune có thể được sử dụng để tạo và triển khai hồ sơ email cho máy khách email gốc (tích hợp) trên nhiều nền tảng thiết bị.</span><span class="sxs-lookup"><span data-stu-id="491a2-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="491a2-104">Để biết thông tin về một số hạn chế liên quan đến hồ sơ email, bao gồm cách xử lý sự hiện diện của các cấu hình hiện có và cách xóa hồ sơ email, hãy xem [Thêm cài đặt email vào thiết bị bằng InTune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="491a2-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="491a2-105">Để biết thêm thông tin về cách tạo hồ sơ email cho từng nền tảng thiết bị, xem:</span><span class="sxs-lookup"><span data-stu-id="491a2-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="491a2-106">Cài đặt thiết bị Android để đặt cấu hình email, xác thực và đồng bộ hoá trong InTune</span><span class="sxs-lookup"><span data-stu-id="491a2-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="491a2-107">Thêm cài đặt e-mail cho các thiết bị iOS và iPadOS trong Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="491a2-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="491a2-108">Cài đặt cấu hình email trong Microsoft InTune cho các thiết bị chạy Windows Phone 8,1</span><span class="sxs-lookup"><span data-stu-id="491a2-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="491a2-109">Cài đặt cấu hình email cho các thiết bị chạy Windows 10 trong Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="491a2-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="491a2-110">**Vấn đề đồng bộ hoá phổ biến**</span><span class="sxs-lookup"><span data-stu-id="491a2-110">**Common syncing issue**</span></span>

<span data-ttu-id="491a2-111">**Một KNOX trên hồ sơ email Android ngăn người dùng liên hệ, lịch và tác vụ, từ đang được đồng bộ với thiết bị người dùng.**</span><span class="sxs-lookup"><span data-stu-id="491a2-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="491a2-112">KNOX trên hồ sơ email Android KNOX cung cấp quản trị tùy chọn để quyết định loại nội dung nào đang đồng bộ hóa với thiết bị bằng cách đặt từng bật.</span><span class="sxs-lookup"><span data-stu-id="491a2-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="491a2-113">Nếu cài đặt cho bất kỳ loại nội dung nào được đặt thành **không cấu hình** (mặc định), loại nội dung đó không đồng bộ tự động.</span><span class="sxs-lookup"><span data-stu-id="491a2-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="491a2-114">Người dùng có thể kích hoạt loại nội dung mà họ muốn trực tiếp trên thiết bị theo cách thủ công, nhưng cấu hình đó được ghi đè bởi thiết đặt chính sách InTune và dừng đồng bộ hóa cho loại nội dung đó.</span><span class="sxs-lookup"><span data-stu-id="491a2-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

