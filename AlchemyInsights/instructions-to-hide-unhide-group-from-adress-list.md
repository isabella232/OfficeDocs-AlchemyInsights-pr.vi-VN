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
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Ẩn Microsoft 365 nhóm từ danh sách địa chỉ (GAL)

Để ẩn một nhóm Microsoft 365 từ danh sách địa chỉ (GAL) của khách hàng Exchange (chẳng hạn như Outlook hoặc OWA), sử dụng các lệnh trong EXO vỏ:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Để ẩn nhóm Microsoft 365 được hiển thị cho khách hàng Exchange, sử dụng các lệnh trong EXO vỏ:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

