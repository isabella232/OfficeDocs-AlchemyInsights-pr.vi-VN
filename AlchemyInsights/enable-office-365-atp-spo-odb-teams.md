---
title: Cho phép Office 365 ATP dành cho SharePoint, OneDrive và Microsoft teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506940"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="fa5e4-102">Cho phép Office 365 nâng cao mối đe dọa bảo vệ cho SharePoint trực tuyến, OneDrive và Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="fa5e4-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="fa5e4-103">Đi tới https://protection.office.com và đăng nhập.</span><span class="sxs-lookup"><span data-stu-id="fa5e4-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="fa5e4-104">Chọn **mối đe dọa quản lý**  >  **chính sách**  >  **đính kèm an toàn**.</span><span class="sxs-lookup"><span data-stu-id="fa5e4-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="fa5e4-105">Chọn **bật ATP cho SharePoint, OneDrive và Microsoft teams**, sau đó bấm vào **lưu**.</span><span class="sxs-lookup"><span data-stu-id="fa5e4-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="fa5e4-106">Khuyến cáo Là quản trị viên toàn cầu hoặc quản trị viên SharePoint trực tuyến, chạy lệnh ghép ngắn [Set-Spothuê](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) với tham số **Disallowinfectedfiledownload** đặt *đúng*.</span><span class="sxs-lookup"><span data-stu-id="fa5e4-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="fa5e4-107">Khuyến cáo [Thiết lập cảnh báo](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) cho các tệp được phát hiện.</span><span class="sxs-lookup"><span data-stu-id="fa5e4-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="fa5e4-108">ATP sẽ NTO quét mọi tệp duy nhất trong SharePoint Online, OneDrive hoặc Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="fa5e4-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="fa5e4-109">Tập tin được quét không đồng bộ, thông qua một quá trình sử dụng chia sẻ và các sự kiện hoạt động khách, cùng với thông minh chẩn đoán và mối đe dọa tín hiệu để xác định các tập tin độc hại.</span><span class="sxs-lookup"><span data-stu-id="fa5e4-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="fa5e4-110">Xem [ATP cho SharePoint, OneDrive và Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="fa5e4-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>