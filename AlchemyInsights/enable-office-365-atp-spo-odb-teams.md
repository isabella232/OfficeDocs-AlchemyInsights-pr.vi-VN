---
title: Cho phép Office 365 ATP cho SharePoint, OneDrive và Microsoft nhóm
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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801097"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="ed3c7-102">Cho phép Microsoft Defender cho Office 365 cho SharePoint Online, OneDrive và Microsoft nhóm</span><span class="sxs-lookup"><span data-stu-id="ed3c7-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="ed3c7-103">Đi đến https://protection.office.com và đăng nhập.</span><span class="sxs-lookup"><span data-stu-id="ed3c7-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="ed3c7-104">Chọn chính sách **quản lý mối đe dọa**  >  **Policy**  >  **an toàn phần đính kèm** .</span><span class="sxs-lookup"><span data-stu-id="ed3c7-104">Choose **Threat management** > **Policy** > **Safe Attachments** .</span></span>
3. <span data-ttu-id="ed3c7-105">Chọn **bật ATP cho SharePoint, OneDrive và Microsoft nhóm** , rồi bấm **lưu** .</span><span class="sxs-lookup"><span data-stu-id="ed3c7-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams** , and then click **Save** .</span></span>
4. <span data-ttu-id="ed3c7-106">Quản Với tư cách là người quản trị toàn cầu hoặc người quản trị SharePoint Online, hãy chạy lệnh ghép ngắn [Set-spođối](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) với bộ tham số **tải xuống của Outallowinfectedfileto** *True* .</span><span class="sxs-lookup"><span data-stu-id="ed3c7-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true* .</span></span>
5. <span data-ttu-id="ed3c7-107">Quản [Thiết lập cảnh báo](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) cho các tệp đã phát hiện.</span><span class="sxs-lookup"><span data-stu-id="ed3c7-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="ed3c7-108">ATP sẽ NTO quét tất cả tệp đơn lẻ trong SharePoint Online, OneDrive hoặc Microsoft nhóm.</span><span class="sxs-lookup"><span data-stu-id="ed3c7-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="ed3c7-109">Các tệp được quét asynchronously, qua một quy trình sử dụng các sự kiện hoạt động chia sẻ và khách, cùng với các tín hiệu thông minh và phản đối mối đe dọa để xác định các tệp độc hại.</span><span class="sxs-lookup"><span data-stu-id="ed3c7-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="ed3c7-110">Xem [ATP cho SharePoint, OneDrive và Microsoft nhóm](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="ed3c7-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>