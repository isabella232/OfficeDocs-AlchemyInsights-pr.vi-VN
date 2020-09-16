---
title: Đặt hoặc thay đổi quyền đối với thư mục công cộng
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: c035d56ffade45cc4360a1d0dfca4c63bf110a38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771214"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="91d87-102">Các quyền và thư mục công cộng</span><span class="sxs-lookup"><span data-stu-id="91d87-102">Permissions and Public Folders</span></span>

<span data-ttu-id="91d87-103">Bạn có thể thay đổi quyền trên thư mục công cộng của bạn bằng cách dùng Outlook, Trung tâm quản trị Exchange (EAC) hoặc PowerShell:</span><span class="sxs-lookup"><span data-stu-id="91d87-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="91d87-104">Đối với hướng dẫn về Outlook, [hãy bấm vào đây](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="91d87-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="91d87-105">Đối với EAC, hãy tham khảo [bài viết này](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) để biết hướng dẫn.</span><span class="sxs-lookup"><span data-stu-id="91d87-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="91d87-106">Đối với PowerShell, hãy tham khảo [bài viết này](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) để biết hướng dẫn về cách sử dụng lệnh ghép ngắn Add-Publicfolderpermission.</span><span class="sxs-lookup"><span data-stu-id="91d87-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="91d87-107">Nếu bạn cần hướng dẫn để kết nối với Exchange PowerShell, hãy bấm vào [đây](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="91d87-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="91d87-108">Nếu **người dùng bên ngoài không thể gửi email đến thư mục công cộng cho phép thư**, lý do có thể là thư mục công cộng bị thiếu quyền cần thiết để chuyển phát email bên ngoài.</span><span class="sxs-lookup"><span data-stu-id="91d87-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="91d87-109">Bạn có thể khắc phục sự cố này bằng cách sử dụng hướng dẫn trong Outlook [tại đây](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)hoặc hướng dẫn PowerShell [tại đây](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="91d87-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

