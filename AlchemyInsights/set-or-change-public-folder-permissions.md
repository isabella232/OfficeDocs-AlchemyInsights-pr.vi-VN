---
title: Đặt hoặc thay đổi quyền thư mục chung
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: cf891a4db05b8a2bdb223cc86693f5072faca494
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43681126"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="16e2d-102">Quyền và thư mục công cộng</span><span class="sxs-lookup"><span data-stu-id="16e2d-102">Permissions and Public Folders</span></span>

<span data-ttu-id="16e2d-103">Bạn có thể thay đổi quyền trên thư mục công cộng của bạn bằng cách sử dụng Outlook, Trung tâm quản trị Exchange (EAC) hoặc PowerShell:</span><span class="sxs-lookup"><span data-stu-id="16e2d-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="16e2d-104">Đối với hướng dẫn Outlook, [Bấm vào đây](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="16e2d-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="16e2d-105">Đối với EAC, hãy tham khảo [bài viết này](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) để biết hướng dẫn.</span><span class="sxs-lookup"><span data-stu-id="16e2d-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="16e2d-106">Đối với PowerShell, hãy tham khảo [bài viết này](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) để biết hướng dẫn về cách sử dụng Commandfolderclientpermission thêm.</span><span class="sxs-lookup"><span data-stu-id="16e2d-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="16e2d-107">Nếu bạn cần hướng dẫn để kết nối với Exchange PowerShell, bấm vào [đây](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="16e2d-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="16e2d-108">Nếu **người dùng bên ngoài không thể gửi email thư mục công cộng kích hoạt thư**, lý do có thể là thư mục công cộng thiếu quyền cần thiết để gửi email bên ngoài.</span><span class="sxs-lookup"><span data-stu-id="16e2d-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="16e2d-109">Bạn có thể khắc phục sự cố này bằng cách sử dụng hướng dẫn Outlook [ở đây](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)hoặc hướng dẫn PowerShell [ở đây](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="16e2d-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

