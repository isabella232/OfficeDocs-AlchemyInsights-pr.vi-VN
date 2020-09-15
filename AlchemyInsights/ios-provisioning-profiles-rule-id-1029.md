---
title: ID quy tắc hồ sơ cung cấp iOS 1029
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "322"
- "3100011"
ms.assetid: 14d30092-8cf5-4fe6-a2a3-8a337e96cb1c
ms.openlocfilehash: a571261ffcb327da50832bc5cb7169b769c2122c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695815"
---
# <a name="ios-provisioning-profiles"></a><span data-ttu-id="241dd-102">Các hồ sơ cung cấp iOS</span><span class="sxs-lookup"><span data-stu-id="241dd-102">iOS Provisioning Profiles</span></span>

<span data-ttu-id="241dd-103">Apple iOS line-of-Business dùng khái niệm về một hồ sơ cung cấp được dùng để xác thực tính toàn vẹn của ứng dụng và thực thi các chính sách được xác định trong hồ sơ.</span><span class="sxs-lookup"><span data-stu-id="241dd-103">Apple iOS line-of-business uses the concept of a provisioning profile which is used to validate the integrity of the application and enforce policies defined in the profile.</span></span> <span data-ttu-id="241dd-104">Các hồ sơ cung cấp này sẽ hết hạn sau 12 tháng và vì vậy một hồ sơ mới phải được liên kết với ứng dụng đã triển khai để các ứng dụng tiếp tục chạy.</span><span class="sxs-lookup"><span data-stu-id="241dd-104">These provisioning profiles expire after 12 months and so a new profile must be associated with the deployed app in order for the apps to continue to to run.</span></span>
  
<span data-ttu-id="241dd-105">Bài viết sau mô tả cách tạo liên kết một hồ sơ cung cấp mới với ứng dụng iOS LOB được triển khai thông qua InTune: [dùng hồ sơ cung cấp ứng dụng iOS để ngăn không cho ứng dụng của bạn hết](https://docs.microsoft.com/intune/app-provisioning-profile-ios) hạn</span><span class="sxs-lookup"><span data-stu-id="241dd-105">The following article describes how to create associate a new provisioning profile with an iOS LOB app deployed through Intune: [Use iOS app provisioning profiles to prevent your apps from expiring](https://docs.microsoft.com/intune/app-provisioning-profile-ios)</span></span>
  