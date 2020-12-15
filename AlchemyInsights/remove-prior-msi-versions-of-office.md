---
title: Loại bỏ các phiên bản MSI trước đó của Office
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680781"
---
# <a name="remove-prior-msi-versions-of-office"></a><span data-ttu-id="52f0e-102">Loại bỏ các phiên bản MSI trước đó của Office</span><span class="sxs-lookup"><span data-stu-id="52f0e-102">Remove prior MSI versions of Office</span></span>

<span data-ttu-id="52f0e-103">Tôi khuyên bạn nên loại bỏ phiên bản Windows Installer (MSI) trước khi cài đặt Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="52f0e-103">I recommend removing prior Windows Installer (MSI) versions of Office before installing Office 365 ProPlus.</span></span> <span data-ttu-id="52f0e-104">Sau đây là cách thực hiện:</span><span class="sxs-lookup"><span data-stu-id="52f0e-104">Here's how to do this:</span></span>

1. <span data-ttu-id="52f0e-105">Nếu bạn đã sử dụng MSI để cài đặt Office, bạn có thể sử dụng công cụ triển khai Office (ODT) để gỡ cài đặt Office.</span><span class="sxs-lookup"><span data-stu-id="52f0e-105">If you used MSI to install Office, you can use the Office Deployment Tool (ODT) to uninstall Office.</span></span> <span data-ttu-id="52f0e-106">Bạn có thể sử dụng phần tử RemoveMSI trong tệp **configuration.xml** của bạn.</span><span class="sxs-lookup"><span data-stu-id="52f0e-106">You can use the RemoveMSI element in your **configuration.xml** file.</span></span>
1. <span data-ttu-id="52f0e-107">Làm theo hướng dẫn trong bài viết này: [Trung tâm tuân thủ & bảo mật của Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="52f0e-107">Follow the instruction in this article: [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span></span>