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
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908366"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="ae2ff-102">Ẩn Microsoft 365 nhóm từ danh sách địa chỉ (GAL)</span><span class="sxs-lookup"><span data-stu-id="ae2ff-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="ae2ff-103">Để ẩn một nhóm Microsoft 365 từ danh sách địa chỉ (GAL) của khách hàng Exchange (chẳng hạn như Outlook hoặc OWA), sử dụng các lệnh trong EXO vỏ:</span><span class="sxs-lookup"><span data-stu-id="ae2ff-103">To hide an Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="ae2ff-104">Để ẩn nhóm Microsoft 365 được hiển thị cho khách hàng Exchange, sử dụng các lệnh trong EXO vỏ:</span><span class="sxs-lookup"><span data-stu-id="ae2ff-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

