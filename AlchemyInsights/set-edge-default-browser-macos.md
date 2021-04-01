---
title: Đặt Microsoft Edge làm trình duyệt mặc định trên thiết bị macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491820"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="4d2bd-102">Đặt Microsoft Edge làm trình duyệt mặc định trên thiết bị macOS</span><span class="sxs-lookup"><span data-stu-id="4d2bd-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="4d2bd-103">Sử dụng một trong hai phương pháp sau đây để đặt Microsoft Edge làm trình duyệt mặc định:</span><span class="sxs-lookup"><span data-stu-id="4d2bd-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="4d2bd-104">Phương pháp 1: flash thiết bị với một hình ảnh macOS mà Microsoft Edge đã được đặt làm trình duyệt mặc định.</span><span class="sxs-lookup"><span data-stu-id="4d2bd-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="4d2bd-105">Phương pháp 2: đặt chính sách DefaultBrowserSettingEnabled để nhắc người dùng đặt Microsoft Edge làm trình duyệt mặc định.</span><span class="sxs-lookup"><span data-stu-id="4d2bd-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="4d2bd-106">Phương pháp cho phép người dùng thay đổi trình duyệt mặc định.</span><span class="sxs-lookup"><span data-stu-id="4d2bd-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="4d2bd-107">Vì lý do này, chúng tôi khuyên bạn nên triển khai chính sách DefaultBrowserSettingEnabled ngay cả khi bạn đã sử dụng phương pháp 1.</span><span class="sxs-lookup"><span data-stu-id="4d2bd-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="4d2bd-108">Nếu người dùng thay đổi trình duyệt mặc định sau khi triển khai chính sách, chính sách sẽ nhắc người dùng thiết lập trình duyệt mặc định trở về Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="4d2bd-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
