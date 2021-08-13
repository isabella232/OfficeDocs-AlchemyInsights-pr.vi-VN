---
title: Hướng dẫn ẩn/bỏ ẩn nhóm khỏi danh sách địa chỉ
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
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926267"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Ẩn Microsoft 365 nhóm khỏi danh sách địa chỉ (GAL)

Để ẩn một nhóm Microsoft 365 khỏi danh sách địa chỉ (GAL) của máy khách Exchange (chẳng hạn như Outlook hoặc OWA), hãy sử dụng lệnh sau đây trong EXO shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Để ẩn nhóm Microsoft 365 ẩn cho máy khách Exchange khách, hãy sử dụng lệnh sau đây trong EXO shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

