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
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Ẩn nhóm Microsoft 365 khỏi danh sách địa chỉ (GAL)

Để ẩn một nhóm Microsoft 365 từ danh sách địa chỉ (GAL) của máy khách Exchange (chẳng hạn như Outlook hoặc OWA), hãy dùng lệnh sau trong EXO Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Để ẩn nhóm Microsoft 365 không thể hiển thị với máy khách Exchange, hãy dùng lệnh sau trong EXO Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

