---
title: Hướng dẫn ẩn/hủy ẩn nhóm từ danh sách địa chỉ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831900"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="72a59-102">Ẩn nhóm Microsoft 365 khỏi danh sách địa chỉ (GAL)</span><span class="sxs-lookup"><span data-stu-id="72a59-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="72a59-103">Để ẩn một nhóm Microsoft 365 từ danh sách địa chỉ (GAL) của máy khách Exchange (chẳng hạn như Outlook hoặc OWA), hãy dùng lệnh sau trong EXO Shell:</span><span class="sxs-lookup"><span data-stu-id="72a59-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="72a59-104">Để ẩn nhóm Microsoft 365 không thể hiển thị với máy khách Exchange, hãy dùng lệnh sau trong EXO Shell:</span><span class="sxs-lookup"><span data-stu-id="72a59-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

