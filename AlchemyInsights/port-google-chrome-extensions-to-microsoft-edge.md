---
title: Các phần mở rộng của cổng Google Chrome vào Microsoft Edge (Crom)
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
ms.openlocfilehash: 1c71d74d01c1e38e4c7789aea2c0b43701b3a5de
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505306"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="088f1-102">Các phần mở rộng của cổng Google Chrome vào Microsoft Edge (Crom)</span><span class="sxs-lookup"><span data-stu-id="088f1-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="088f1-103">Thật dễ dàng để [mở rộng cổng Google Chrome sang Microsoft Edge (Crom)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span><span class="sxs-lookup"><span data-stu-id="088f1-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="088f1-104">Trong hầu hết các trường hợp, chỉ cần những thay đổi tối thiểu để chạy các phần mở rộng này trên Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="088f1-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="088f1-105">Các API mở rộng và các phím Hiển thị được hỗ trợ bởi Google Chrome là mã tương thích với Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="088f1-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="088f1-106">Tuy nhiên, Microsoft Edge không hỗ trợ phần mở rộng API Chrome. GCM, Chrome. Identity. getAccounts, Chrome. Identity. getAuthToken và Chrome. instanceID.</span><span class="sxs-lookup"><span data-stu-id="088f1-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>