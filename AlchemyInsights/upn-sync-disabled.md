---
title: Đồng bộ UPN bị vô hiệu hóa
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
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749536"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="eb0cc-102">Đồng bộ UPN bị vô hiệu hóa</span><span class="sxs-lookup"><span data-stu-id="eb0cc-102">UPN sync disabled</span></span>

<span data-ttu-id="eb0cc-103">Nếu bạn đã bắt đầu đồng bộ với Azure AD trước ngày 30 tháng 3, 2016, hãy chạy lệnh ghép ngắn Azure AD PowerShell sau đây để bật khớp với khớp mềm UPN cho tổ chức của bạn:</span><span class="sxs-lookup"><span data-stu-id="eb0cc-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="eb0cc-104">**Thiết lập-MsolDirSyncFeature-tính năng EnableSoftMatchOnUpn-bật $True**</span><span class="sxs-lookup"><span data-stu-id="eb0cc-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="eb0cc-105">Khớp mềm UPN được tự động bật cho các tổ chức bắt đầu đồng bộ với Azure AD vào hoặc sau ngày 30 tháng 3, 2016.</span><span class="sxs-lookup"><span data-stu-id="eb0cc-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="eb0cc-106">Để tìm hiểu thêm về việc bật tính năng khớp mềm trên UPN và các tính năng đồng bộ khác, vui lòng xem [AZURE AD Connect Sync Service](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="eb0cc-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

