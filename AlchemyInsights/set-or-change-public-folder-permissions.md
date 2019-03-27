---
title: Thiết lập hoặc thay đổi quyền truy cập thư mục chung
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: d1554e8a63455f3549044e526183c0e8709f2631
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767306"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="9b26e-102">Quyền hạn và thư mục công cộng</span><span class="sxs-lookup"><span data-stu-id="9b26e-102">Permissions and Public Folders</span></span>

<span data-ttu-id="9b26e-103">Bạn có thể thay đổi các cấp phép trên cặp công cộng của bạn bằng cách sử dụng Outlook, Trung tâm quản trị Exchange (EAC), hoặc PowerShell:</span><span class="sxs-lookup"><span data-stu-id="9b26e-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="9b26e-104">Outlook hướng dẫn, [Bấm vào đây](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="9b26e-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="9b26e-105">Để EAC, tham khảo [bài viết này](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) để được hướng dẫn.</span><span class="sxs-lookup"><span data-stu-id="9b26e-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> <span data-ttu-id="9b26e-106">Bạn có thể bấm vào [đây](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) để điều hướng đến EAC.</span><span class="sxs-lookup"><span data-stu-id="9b26e-106">You can click [here](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) to navigate to EAC.</span></span> 
    
- <span data-ttu-id="9b26e-107">Cho Powershell, hãy tham khảo [bài viết này](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) để biết hướng dẫn về cách sử dụng Add-PublicFolderClientPermission commandlet.</span><span class="sxs-lookup"><span data-stu-id="9b26e-107">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="9b26e-108">Nếu bạn cần hướng dẫn để kết nối với Exchange Powershell, bấm vào [đây](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="9b26e-108">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="9b26e-109">Nếu **người dùng bên ngoài không thể gửi email đến một thư mục công cộng kích hoạt thư**, nguyên nhân có thể được cặp công cộng là thiếu quyền cần thiết để gửi email bên ngoài.</span><span class="sxs-lookup"><span data-stu-id="9b26e-109">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="9b26e-110">Bạn có thể sửa lỗi này bằng cách sử dụng Outlook hướng dẫn [ở đây](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), hoặc hướng dẫn PowerShell [tại đây](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="9b26e-110">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

