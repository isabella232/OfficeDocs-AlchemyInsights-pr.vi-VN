---
title: Chuỗi đại diện người dùng Microsoft Edge (máy tính để bàn)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679328"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="fcc11-102">Chuỗi đại diện người dùng Microsoft Edge (máy tính để bàn)</span><span class="sxs-lookup"><span data-stu-id="fcc11-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="fcc11-103">Chuỗi đại diện người dùng (UA) có thể được dùng để phát hiện phiên bản của một trình duyệt cụ thể đang được sử dụng trên một hệ điều hành nhất định.</span><span class="sxs-lookup"><span data-stu-id="fcc11-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="fcc11-104">Giống như các trình duyệt khác, Microsoft Edge sẽ bao gồm thông tin này trong phần đầu trang "User-Agent" bất cứ khi nào nó tạo một yêu cầu đến một site.</span><span class="sxs-lookup"><span data-stu-id="fcc11-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="fcc11-105">Trình duyệt-thông tin Phiên bản cũng có thể được truy nhập thông qua JavaScript bằng cách truy vấn giá trị của "Navigator. userAgent".</span><span class="sxs-lookup"><span data-stu-id="fcc11-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="fcc11-106">Chúng tôi khuyên bạn nên sử dụng phát hiện tính năng bất cứ khi nào có thể cải thiện khả năng duy trì mã, giảm bớt độ mong manh của mã và loại bỏ nguy cơ vỡ mã trong trường hợp các bản Cập Nhật chuỗi tương lai của UA.</span><span class="sxs-lookup"><span data-stu-id="fcc11-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="fcc11-107">Để biết thêm thông tin, hãy xem [chuỗi đại diện người dùng Microsoft Edge (màn hình máy tính)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span><span class="sxs-lookup"><span data-stu-id="fcc11-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>