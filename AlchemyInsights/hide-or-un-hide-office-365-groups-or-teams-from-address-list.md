---
title: Ẩn hoặc bỏ ẩn nhóm Office 365 hoặc nhóm từ danh sách địa chỉ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811478"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Ẩn hoặc bỏ ẩn nhóm Office 365 hoặc nhóm từ danh sách địa chỉ

Sử dụng lệnh EXO PowerShell sau đây để ẩn hoặc bỏ ẩn nhóm Office 365/nhóm từ danh sách địa chỉ (GAL) của máy khách Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Sử dụng lệnh EXO PowerShell sau đây để ẩn hoặc bỏ ẩn nhóm Office365 từ Exchange Client (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Để biết hướng dẫn chi tiết, hãy xem [ẩn các nhóm Office 365 từ máy khách gal và Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
