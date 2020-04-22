---
title: Đồng bộ hoá UPN tắt
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
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726126"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="767d9-102">Đồng bộ hoá UPN tắt</span><span class="sxs-lookup"><span data-stu-id="767d9-102">UPN sync disabled</span></span>

<span data-ttu-id="767d9-103">Nếu bạn bắt đầu đồng bộ hoá Azure AD trước ngày 30 tháng 2016, chạy lệnh Azure AD PowerShell sau để cho phép UPN mềm phù hợp cho tổ chức của bạn chỉ:</span><span class="sxs-lookup"><span data-stu-id="767d9-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="767d9-104">**Thiết lập MsolDirSyncFeature-tính năng EnableSoftMatchOnUpn-kích hoạt $True**</span><span class="sxs-lookup"><span data-stu-id="767d9-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="767d9-105">UPN mềm phù hợp tự động bật cho các tổ chức bắt đầu đồng bộ hoá quảng cáo Azure vào hoặc sau ngày 30 tháng 3 năm 2016.</span><span class="sxs-lookup"><span data-stu-id="767d9-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="767d9-106">Để tìm hiểu thêm về cho phép khớp mềm trên UPN và các tính năng đồng bộ hoá khác, vui lòng xem [tính năng dịch vụ đồng bộ hóa AZURE AD kết nối](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="767d9-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

