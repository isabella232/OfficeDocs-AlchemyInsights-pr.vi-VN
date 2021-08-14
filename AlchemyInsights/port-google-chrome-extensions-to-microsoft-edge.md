---
title: Nối cổng tiện ích mở rộng của Google Chrome Microsoft Edge (Chromium)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
- "8297"
- "9004617"
ms.openlocfilehash: 34ec7e71a2f27eb5b46395876a4d1c903189be1050e523796c9f2a817c20aaa0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973719"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Nối cổng tiện ích mở rộng của Google Chrome Microsoft Edge (Chromium)

Thật dễ dàng để nối [cổng phần mở rộng của Google Chrome sang điện Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension). Trong hầu hết các trường hợp, chỉ cần thay đổi tối thiểu để chạy các phần mở rộng này trên Microsoft Edge.

API mở rộng và khóa hiển thị được Google Chrome hỗ trợ tương thích với mã Microsoft Edge. Tuy nhiên, Microsoft Edge không hỗ trợ phần mở rộng API chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken và chrome.instanceID.