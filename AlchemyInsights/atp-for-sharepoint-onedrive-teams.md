---
title: ATP cho SharePoint, OneDrive và Microsoft nhóm
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715583"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="a8d89-102">ATP cho SharePoint, OneDrive và Microsoft nhóm</span><span class="sxs-lookup"><span data-stu-id="a8d89-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="a8d89-103">Làm theo các bước sau để bật tính năng bảo vệ mối đe dọa nâng cao:</span><span class="sxs-lookup"><span data-stu-id="a8d89-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="a8d89-104">Đi đến [https://protection.office.com](https://protection.office.com) và đăng nhập bằng tài khoản người quản trị toàn cầu hoặc người quản trị bảo mật.</span><span class="sxs-lookup"><span data-stu-id="a8d89-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="a8d89-105">Trong ngăn dẫn hướng bên trái bên dưới **quản lý mối đe dọa**, hãy chọn **chính sách** \> **tệp đính kèm an toàn**.</span><span class="sxs-lookup"><span data-stu-id="a8d89-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="a8d89-106">Chọn **bật ATP cho SharePoint, OneDrive và Microsoft nhóm**.</span><span class="sxs-lookup"><span data-stu-id="a8d89-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="a8d89-107">[Tạo một chính sách cảnh báo hoạt động](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) để nhận thông báo khi chúng tôi phát hiện tệp độc hại.</span><span class="sxs-lookup"><span data-stu-id="a8d89-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="a8d89-108">Để biết hướng dẫn đầy đủ, hãy xem [chủ đề](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)này.</span><span class="sxs-lookup"><span data-stu-id="a8d89-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="a8d89-109">**Lưu ý**: theo thiết kế, ATP không quét tất cả tệp duy nhất trong SharePoint Online, OneDrive for Business hoặc Microsoft nhóm.</span><span class="sxs-lookup"><span data-stu-id="a8d89-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="a8d89-110">Các tệp được quét asynchronously theo quy trình sử dụng tính năng chia sẻ hoạt động, hoạt động của khách và các tín hiệu mối đe dọa để xác định các tệp độc hại.</span><span class="sxs-lookup"><span data-stu-id="a8d89-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="a8d89-111">Để biết thêm thông tin, hãy xem [chủ đề](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)này.</span><span class="sxs-lookup"><span data-stu-id="a8d89-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
