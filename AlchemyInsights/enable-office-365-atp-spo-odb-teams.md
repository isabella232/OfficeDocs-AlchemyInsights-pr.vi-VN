---
title: Kích hoạt Office 365 ATP cho SharePoint, OneDrive và Microsoft đội
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/02/2019
ms.locfileid: "31031142"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="73a6e-102">Sử Office 365 nâng cao mối đe dọa bảo vệ cho SharePoint trực tuyến, OneDrive và Microsoft đội</span><span class="sxs-lookup"><span data-stu-id="73a6e-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="73a6e-103">Đi đến https://protection.office.com và đăng nhập.</span><span class="sxs-lookup"><span data-stu-id="73a6e-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="73a6e-104">Chọn **quản lý mối đe dọa** > **chính sách** > **Tập tin đính kèm an toàn**.</span><span class="sxs-lookup"><span data-stu-id="73a6e-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="73a6e-105">Chọn **bật ATP cho Microsoft đội, SharePoint và OneDrive,** và sau đó nhấp vào **lưu**.</span><span class="sxs-lookup"><span data-stu-id="73a6e-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="73a6e-106">(Khuyến cáo) Như là một quản trị toàn cầu hoặc quản trị viên SharePoint Online, chạy lệnh ghép ngắn [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) với tham số **DisallowInfectedFileDownload** được đặt thành *true*.</span><span class="sxs-lookup"><span data-stu-id="73a6e-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="73a6e-107">(Khuyến cáo) [Thiết lập cảnh báo](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) cho các tập tin được phát hiện.</span><span class="sxs-lookup"><span data-stu-id="73a6e-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="73a6e-108">ATP sẽ nto quét mỗi tập tin trong SharePoint Online, OneDrive hoặc Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="73a6e-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="73a6e-109">Tập tin được quét không đồng bộ, thông qua một quá trình sử dụng chia sẻ và khách hoạt động sự kiện, cùng với các chẩn đoán thông minh và mối đe dọa tín hiệu để xác định các tập tin độc hại.</span><span class="sxs-lookup"><span data-stu-id="73a6e-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="73a6e-110">Xem [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="73a6e-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>