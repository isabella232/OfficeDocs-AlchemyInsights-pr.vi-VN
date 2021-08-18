---
title: Ẩn hoặc bỏ ẩn danh sách Office 365 nhóm hoặc nhóm khỏi danh sách địa chỉ
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
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088418"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Ẩn hoặc bỏ ẩn danh sách Office 365 nhóm hoặc nhóm khỏi danh sách địa chỉ

Sử dụng lệnh EXO PowerShell sau đây để ẩn hoặc bỏ ẩn Office 365/nhóm khỏi danh sách địa chỉ (GAL) của máy khách Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Sử dụng lệnh EXO PowerShell sau đây để ẩn hoặc bỏ ẩn nhóm/nhóm Office365 khỏi máy Exchange khách (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Để biết hướng dẫn chi tiết, [hãy xem Office 365 Nhóm Mới khỏi GAL và Exchange Khách hàng.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
