---
title: Bật Office 365 ATP cho tất SharePoint, OneDrive và các Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543950"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="63e28-102">Bật Bộ bảo vệ Microsoft dành Office 365 cho SharePoint Online, OneDrive và Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="63e28-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="63e28-103">Truy nhập https://protection.office.com và đăng nhập.</span><span class="sxs-lookup"><span data-stu-id="63e28-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="63e28-104">Chọn Chính **sách quản lý mối**  >  **đe**  >  **dọa Két sắt phần đính kèm**.</span><span class="sxs-lookup"><span data-stu-id="63e28-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="63e28-105">Chọn **Bật Bộ bảo vệ cho Office 365 cho SharePoint, OneDrive và Microsoft Teams**, sau đó bấm **Lưu**.</span><span class="sxs-lookup"><span data-stu-id="63e28-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="63e28-106">(Được đề xuất) Với tư cách là người quản trị toàn cầu hoặc người quản trị SharePoint Online, hãy chạy lệnh ghép ngắn [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) với tham số **DisallowInfectedFileDownload** được đặt thành *true.*</span><span class="sxs-lookup"><span data-stu-id="63e28-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="63e28-107">(Được đề xuất) [Thiết lập cảnh báo cho các](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) tệp được phát hiện.</span><span class="sxs-lookup"><span data-stu-id="63e28-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="63e28-108">Bộ bảo vệ Microsoft dành Office 365 sẽ không quét từng tệp riêng lẻ trong SharePoint Online, OneDrive hoặc Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="63e28-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="63e28-109">Các tệp được quét không đồng bộ, thông qua một quy trình sử dụng các sự kiện hoạt động chia sẻ và khách, cùng với tín hiệu phân tích thông minh và mối đe dọa để xác định các tệp độc hại.</span><span class="sxs-lookup"><span data-stu-id="63e28-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="63e28-110">Xem [mục Bộ bảo vệ Microsoft Office 365 để biết SharePoint, OneDrive và Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="63e28-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>