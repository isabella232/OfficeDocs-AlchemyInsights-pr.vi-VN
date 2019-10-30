---
title: Hướng dẫn ẩn/bỏ ẩn nhóm từ danh sách địa chỉ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768964"
---
# <a name="hide-office-365-group-from-address-list-gal"></a><span data-ttu-id="e2ce2-102">Ẩn văn phòng 365 nhóm từ danh sách địa chỉ (GAL)</span><span class="sxs-lookup"><span data-stu-id="e2ce2-102">Hide Office 365 group from address list (GAL)</span></span>

<span data-ttu-id="e2ce2-103">Để ẩn nhóm Office 365 từ danh sách địa chỉ (GAL) của khách hàng Exchange (chẳng hạn như Outlook hoặc OWA), sử dụng các lệnh trong EXO vỏ:</span><span class="sxs-lookup"><span data-stu-id="e2ce2-103">To hide an Office 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="e2ce2-104">Để ẩn nhóm Office 365 được hiển thị cho khách hàng Exchange, sử dụng các lệnh trong EXO vỏ:</span><span class="sxs-lookup"><span data-stu-id="e2ce2-104">To hide the Office 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

