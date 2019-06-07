---
title: ATP cho SharePoint, OneDrive và Microsoft đội
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: b304f6c7d9959e49a8152c03f11c6c864a154ea5
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765542"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="48f0a-102">ATP cho SharePoint, OneDrive và Microsoft đội</span><span class="sxs-lookup"><span data-stu-id="48f0a-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="48f0a-103">Hãy làm theo các bước sau để cho phép nâng cao mối đe dọa bảo vệ:</span><span class="sxs-lookup"><span data-stu-id="48f0a-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="48f0a-104">Đi đến [https://protection.office.com](https://protection.office.com) và đăng nhập bằng một người quản trị toàn cầu hoặc tài khoản quản trị an ninh.</span><span class="sxs-lookup"><span data-stu-id="48f0a-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="48f0a-105">Trong ngăn điều hướng bên trái quản lý **mối đe dọa**, chọn **chính sách** \> **Tập tin đính kèm an toàn**.</span><span class="sxs-lookup"><span data-stu-id="48f0a-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="48f0a-106">Chọn **bật ATP cho Microsoft đội, SharePoint và OneDrive**.</span><span class="sxs-lookup"><span data-stu-id="48f0a-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="48f0a-107">[Tạo một chính sách cảnh báo hoạt động](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) để nhận thông báo khi chúng tôi phát hiện các tập tin độc hại.</span><span class="sxs-lookup"><span data-stu-id="48f0a-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="48f0a-108">Hướng dẫn đầy đủ, xem [chủ đề](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams)này.</span><span class="sxs-lookup"><span data-stu-id="48f0a-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="48f0a-109">**Lưu ý**: theo thiết kế, ATP không quét mỗi tập tin trong SharePoint Online, OneDrive cho doanh nghiệp, hoặc Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="48f0a-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="48f0a-110">Tập tin được quét không đồng bộ của một quá trình sử dụng chia sẻ hoạt động, hoạt động đánh, và mối đe dọa tín hiệu để xác định các tập tin độc hại.</span><span class="sxs-lookup"><span data-stu-id="48f0a-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="48f0a-111">Để biết thêm chi tiết, xem [chủ đề](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)này.</span><span class="sxs-lookup"><span data-stu-id="48f0a-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
