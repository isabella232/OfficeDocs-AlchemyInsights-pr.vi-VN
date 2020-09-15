---
title: Xung đột với SourceAnchor, ProxyAddress, UserPrincipalName
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 877c954bea219cf8d885645cd25e41a5b7bab6fd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713476"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="9ab96-102">Xung đột với SourceAnchor, ProxyAddress, UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9ab96-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="9ab96-103">Nếu bạn nhận được lỗi trong khi đồng bộ hóa chẳng hạn như "một đối tượng được đồng bộ với cùng một ProxyAddress hoặc UserPrincipalName tồn tại trong thư mục của bạn", hãy xem [chẩn đoán và khắc phục các lỗi đồng bộ thuộc tính trùng lặp](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span><span class="sxs-lookup"><span data-stu-id="9ab96-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="9ab96-104">Ngoài ra, hãy cân nhắc việc bật tính năng trùng lặp của Resiliency.</span><span class="sxs-lookup"><span data-stu-id="9ab96-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="9ab96-105">Để biết thêm thông tin, hãy xem mục [đồng bộ hóa định danh và thuộc tính trùng lặp Resiliency](https://aka.ms/duplicateattributeresiliency).</span><span class="sxs-lookup"><span data-stu-id="9ab96-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>