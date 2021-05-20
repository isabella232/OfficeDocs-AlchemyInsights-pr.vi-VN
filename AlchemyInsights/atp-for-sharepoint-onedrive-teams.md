---
title: Bộ bảo vệ Microsoft dành Office 365 cho mọi SharePoint, OneDrive và Microsoft Teams
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
ms.openlocfilehash: 7d2ed7bc4c7d99cd01dadc12e38762903d6d8ab3
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543599"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="a4bfc-102">Bộ bảo vệ Microsoft dành Office 365 cho mọi SharePoint, OneDrive và Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="a4bfc-102">Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="a4bfc-103">Làm theo các bước sau để bật Bộ bảo vệ Microsoft dành cho Office 365:</span><span class="sxs-lookup"><span data-stu-id="a4bfc-103">Follow these steps to enable Microsoft Defender for Office 365:</span></span>

1. <span data-ttu-id="a4bfc-104">Truy nhập và [https://protection.office.com](https://protection.office.com) đăng nhập bằng tài khoản người quản trị toàn cầu hoặc người quản trị bảo mật.</span><span class="sxs-lookup"><span data-stu-id="a4bfc-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="a4bfc-105">Trong ngăn dẫn hướng bên trái bên dưới Quản **lý mối đe dọa**, **chọn Chính** \> **Két sắt kèm**.</span><span class="sxs-lookup"><span data-stu-id="a4bfc-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="a4bfc-106">Chọn **Bật Bộ bảo vệ cho Office 365 cho SharePoint, OneDrive, rồi Microsoft Teams.**</span><span class="sxs-lookup"><span data-stu-id="a4bfc-106">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="a4bfc-107">[Tạo chính sách cảnh báo hoạt động để](/microsoft-365/compliance/create-activity-alerts) nhận thông báo khi chúng tôi phát hiện các tệp độc hại.</span><span class="sxs-lookup"><span data-stu-id="a4bfc-107">[Create an activity alert policy](/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="a4bfc-108">Để biết hướng dẫn đầy đủ, hãy xem mục Bật Két sắt [kèm cho SharePoint, OneDrive và Microsoft Teams.](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="a4bfc-108">For complete instructions, see this [Turn on Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="a4bfc-109">**Lưu** ý: Theo thiết kế, Microsoft Defender dành cho Office 365 không quét từng tệp riêng lẻ trong SharePoint Online, OneDrive for Business hoặc Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a4bfc-109">**Note**: By design, Microsoft Defender for Office 365 doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="a4bfc-110">Các tệp được quét không đồng bộ bằng một quy trình sử dụng hoạt động chia sẻ, hoạt động của khách và tín hiệu mối đe dọa để xác định các tệp độc hại.</span><span class="sxs-lookup"><span data-stu-id="a4bfc-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="a4bfc-111">Để biết thêm thông tin, [hãy xem Két sắt kèm để biết SharePoint, OneDrive và Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="a4bfc-111">For more information, see [Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
