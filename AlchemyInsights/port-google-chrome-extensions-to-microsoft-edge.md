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
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678976"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="3d274-102">Các phần mở rộng của cổng Google Chrome vào Microsoft Edge (Crom)</span><span class="sxs-lookup"><span data-stu-id="3d274-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="3d274-103">Thật dễ dàng để [mở rộng cổng Google Chrome sang Microsoft Edge (Crom)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span><span class="sxs-lookup"><span data-stu-id="3d274-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="3d274-104">Trong hầu hết các trường hợp, chỉ cần những thay đổi tối thiểu để chạy các phần mở rộng này trên Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="3d274-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="3d274-105">Các API mở rộng và các phím Hiển thị được hỗ trợ bởi Google Chrome là mã tương thích với Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="3d274-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="3d274-106">Tuy nhiên, Microsoft Edge không hỗ trợ phần mở rộng API Chrome. GCM, Chrome. Identity. getAccounts, Chrome. Identity. getAuthToken và Chrome. instanceID.</span><span class="sxs-lookup"><span data-stu-id="3d274-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>