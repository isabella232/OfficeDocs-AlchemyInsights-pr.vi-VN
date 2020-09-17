---
title: Ẩn hoặc bỏ ẩn nhóm Office 365 hoặc nhóm từ danh sách địa chỉ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 1204b9f45fe34015f72c559f77674e980d28c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47782349"
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
