---
title: Đồng bộ UPN bị vô hiệu hoá
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532353"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="813bd-102">Đồng bộ UPN bị vô hiệu hoá</span><span class="sxs-lookup"><span data-stu-id="813bd-102">UPN sync disabled</span></span>

<span data-ttu-id="813bd-103">Nếu bạn bắt đầu đồng bộ hoá với các quảng cáo Azure trước ngày 30 tháng 3 năm 2016, chạy lệnh ghép ngắn PowerShell Azure quảng cáo sau đây để sử UPN mềm mại phù hợp cho tổ chức của bạn chỉ:</span><span class="sxs-lookup"><span data-stu-id="813bd-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="813bd-104">**Thiết lập MsolDirSyncFeature-có EnableSoftMatchOnUpn-sử $True**</span><span class="sxs-lookup"><span data-stu-id="813bd-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="813bd-105">UPN mềm phù hợp sẽ được bật cho các tổ chức bắt đầu đồng bộ hoá quảng cáo Azure vào hoặc sau ngày 30 tháng 3 năm 2016.</span><span class="sxs-lookup"><span data-stu-id="813bd-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="813bd-106">Để tìm hiểu thêm về bật mềm trận trên UPN và các tính năng đồng bộ hóa, hãy xem [tính năng dịch vụ Azure quảng cáo kết nối đồng bộ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="813bd-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

