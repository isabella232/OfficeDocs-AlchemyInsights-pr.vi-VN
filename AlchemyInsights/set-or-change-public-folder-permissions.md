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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32421838"
---
# <a name="permissions-and-public-folders"></a>Quyền hạn và thư mục công cộng

Bạn có thể thay đổi các cấp phép trên cặp công cộng của bạn bằng cách sử dụng Outlook, Trung tâm quản trị Exchange (EAC), hoặc PowerShell:
  
- Outlook hướng dẫn, [Bấm vào đây](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).
    
- Để EAC, tham khảo [bài viết này](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) để được hướng dẫn. Bạn có thể bấm vào [đây](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) để điều hướng đến EAC. 
    
- Cho Powershell, hãy tham khảo [bài viết này](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) để biết hướng dẫn về cách sử dụng Add-PublicFolderClientPermission commandlet. Nếu bạn cần hướng dẫn để kết nối với Exchange Powershell, bấm vào [đây](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).
    
Nếu **người dùng bên ngoài không thể gửi email đến một thư mục công cộng kích hoạt thư**, nguyên nhân có thể được cặp công cộng là thiếu quyền cần thiết để gửi email bên ngoài. Bạn có thể sửa lỗi này bằng cách sử dụng Outlook hướng dẫn [ở đây](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), hoặc hướng dẫn PowerShell [tại đây](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).
  

