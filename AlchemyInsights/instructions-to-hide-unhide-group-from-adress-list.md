---
title: Hướng dẫn ẩn/hủy ẩn nhóm từ danh sách địa chỉ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663031"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Ẩn nhóm Microsoft 365 khỏi danh sách địa chỉ (GAL)

Để ẩn một nhóm Microsoft 365 từ danh sách địa chỉ (GAL) của máy khách Exchange (chẳng hạn như Outlook hoặc OWA), hãy dùng lệnh sau trong EXO Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Để ẩn nhóm Microsoft 365 không thể hiển thị với máy khách Exchange, hãy dùng lệnh sau trong EXO Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

