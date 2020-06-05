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
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580031"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="94672-102">Ẩn Microsoft 365 nhóm từ danh sách địa chỉ (GAL)</span><span class="sxs-lookup"><span data-stu-id="94672-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="94672-103">Để ẩn một nhóm Microsoft 365 từ danh sách địa chỉ (GAL) của khách hàng Exchange (chẳng hạn như Outlook hoặc OWA), sử dụng các lệnh trong EXO vỏ:</span><span class="sxs-lookup"><span data-stu-id="94672-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="94672-104">Để ẩn nhóm Microsoft 365 được hiển thị cho khách hàng Exchange, sử dụng các lệnh trong EXO vỏ:</span><span class="sxs-lookup"><span data-stu-id="94672-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

