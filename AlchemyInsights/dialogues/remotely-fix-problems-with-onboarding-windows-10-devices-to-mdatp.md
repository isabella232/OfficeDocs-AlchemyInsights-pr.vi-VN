---
title: Khắc phục sự cố từ xa với các thiết bị chạy Windows 10 cho bộ bảo vệ mối đe dọa nâng cao của Microsoft Defender
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694840"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="8d2e8-102">Khắc phục sự cố từ xa với các thiết bị chạy Windows 10 cho bộ bảo vệ mối đe dọa nâng cao của Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="8d2e8-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="8d2e8-103">Nếu bạn có thể truy nhập vào máy tính từ xa, hãy làm theo các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="8d2e8-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="8d2e8-104">Tải xuống công cụ chẩn đoán [kết nối máy khách](https://go.microsoft.com/fwlink/?linkid=2143466) .</span><span class="sxs-lookup"><span data-stu-id="8d2e8-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="8d2e8-105">Trích xuất và chạy MDATPAnalyzer. cmd.</span><span class="sxs-lookup"><span data-stu-id="8d2e8-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="8d2e8-106">Xác định vị trí Nhật ký chẩn đoán trong thư mục MDATPClientAnalyzerResult, chính là thư mục mà công cụ phân tích đã được tải xuống.</span><span class="sxs-lookup"><span data-stu-id="8d2e8-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="8d2e8-107">Để tìm các vấn đề với kết nối hoặc thiết đặt proxy Internet, hãy xem lại MDATPClientAnalyzer.txt tệp nhật ký.</span><span class="sxs-lookup"><span data-stu-id="8d2e8-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="8d2e8-108">Để tìm hiểu thêm, hãy xem các [vấn đề với máy triển khai](https://go.microsoft.com/fwlink/?linkid=2143634).</span><span class="sxs-lookup"><span data-stu-id="8d2e8-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
