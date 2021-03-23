---
title: Chặn người dùng từ các cuộc họp bản ghi
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037063"
---
# <a name="block-user-from-recording-meetings"></a><span data-ttu-id="01833-102">Chặn người dùng từ các cuộc họp bản ghi</span><span class="sxs-lookup"><span data-stu-id="01833-102">Block User From Recording Meetings</span></span>

<span data-ttu-id="01833-103">Nếu bạn cần **ngăn chặn hoặc chặn** người dùng cụ thể từ các cuộc họp nhóm ghi, bạn có thể làm như vậy thông qua các thiết đặt chính sách cuộc họp nhóm.</span><span class="sxs-lookup"><span data-stu-id="01833-103">If you need to **prevent or block** specific users from recording Teams Meetings, you can do so via Teams Meeting Policy settings.</span></span> <span data-ttu-id="01833-104">Trong Trung tâm quản trị nhóm Microsoft, hãy tắt thiết đặt bản **ghi cho phép đám mây** trong chính sách cuộc họp được gán cho người dùng đó.</span><span class="sxs-lookup"><span data-stu-id="01833-104">In the Microsoft Teams admin center, turn off the **Allow cloud recording** setting in the meeting policy assigned to that user.</span></span> <span data-ttu-id="01833-105">Để tìm hiểu thêm, hãy xem [quản lý chính sách cuộc họp trong nhóm](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span><span class="sxs-lookup"><span data-stu-id="01833-105">To learn more, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span></span>

<span data-ttu-id="01833-106">Để xác thực nếu một người dùng cụ thể được phép hoặc không ghi lại cuộc họp nhóm, hãy sử dụng chẩn đoán hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="01833-106">To validate if a specific user is allowed or not to record Teams Meetings, use the support diagnostic.</span></span> <span data-ttu-id="01833-107">Chạy truy vấn hỗ trợ mới và nhập vào **Diag: bản ghi cuộc họp** -chẩn đoán sẽ kiểm tra các thiết đặt chính sách cho người dùng được chỉ định và xác định các thiết đặt chính sách của họ.</span><span class="sxs-lookup"><span data-stu-id="01833-107">Run a new support query and type in **Diag: Meeting Recording** - the diagnostic will check policy settings for the specified user and determine their policy settings.</span></span> <span data-ttu-id="01833-108">Hãy nhớ rằng, có thể mất một vài giờ để các thiết đặt chính sách mới có hiệu lực, vì vậy nếu bạn vừa thực hiện thay đổi, hãy chờ một vài giờ trước khi chạy lại chẩn đoán.</span><span class="sxs-lookup"><span data-stu-id="01833-108">Remember, it can take a couple of hours for new policy settings to take effect, so if you have just made a change, wait a few hours before running the diagnostic again.</span></span>

<span data-ttu-id="01833-109">Để biết thêm thông tin, hãy xem lại bật hoặc tắt tính năng [ghi đám mây](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span><span class="sxs-lookup"><span data-stu-id="01833-109">For more information, review [Turn on or turn off cloud recording](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span></span>
