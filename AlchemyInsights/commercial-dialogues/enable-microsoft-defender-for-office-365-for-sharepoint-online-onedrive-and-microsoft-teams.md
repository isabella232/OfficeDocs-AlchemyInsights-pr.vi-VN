---
title: Bật Microsoft Defender cho Office 365 cho SharePoint Online, OneDrive và Microsoft nhóm
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747735"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="19518-102">Bật Microsoft Defender cho Office 365 cho SharePoint Online, OneDrive và Microsoft nhóm</span><span class="sxs-lookup"><span data-stu-id="19518-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="19518-103">Sử dụng danh mục quản trị toàn cầu hoặc thông tin xác thực của người quản trị bảo mật, hãy đăng nhập vào [Trung tâm bảo mật và tuân thủ của Office 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="19518-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="19518-104">Chọn **quản lý mối đe dọa** trong ngăn bên trái, rồi chọn **chính sách**  >  [tệp đính kèm an toàn](https://protection.office.com/safeattachment).</span><span class="sxs-lookup"><span data-stu-id="19518-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="19518-105">Chọn **bật Microsoft Defender cho Office 365 cho SharePoint, OneDrive và Microsoft nhóm**, rồi chọn **lưu**.</span><span class="sxs-lookup"><span data-stu-id="19518-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="19518-106">Với tư cách là người quản trị toàn cầu hoặc người quản trị SharePoint Online, hãy chạy lệnh ghép ngắn PowerShell sau đây để đặt tham số **tải xuống** dành cho các đối tượng là *True*: [Set-spothuê](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="19518-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="19518-107">Thiết lập cảnh báo cho các tệp đã phát hiện</span><span class="sxs-lookup"><span data-stu-id="19518-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="19518-108">Để biết thêm thông tin, hãy xem mục [Microsoft Defender dành cho Office 365 cho SharePoint, OneDrive và các nhóm Microsoft](https://go.microsoft.com/fwlink/?linkid=2092041).</span><span class="sxs-lookup"><span data-stu-id="19518-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
