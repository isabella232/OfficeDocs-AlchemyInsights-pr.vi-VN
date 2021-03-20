---
title: Các vấn đề với máy triển khai vào Microsoft Defender cho các điểm cuối
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901589"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="01c50-102">Các vấn đề với máy triển khai vào Microsoft Defender cho các điểm cuối</span><span class="sxs-lookup"><span data-stu-id="01c50-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="01c50-103">Bạn có thể gặp sự cố với máy triển khai vào dịch vụ MDE.</span><span class="sxs-lookup"><span data-stu-id="01c50-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="01c50-104">Nếu bạn có thể truy nhập vào máy người dùng cuối, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="01c50-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="01c50-105">Tải xuống phiên bản xem trước mới nhất của công cụ chẩn đoán [máy khách MDE](https://aka.ms/betamdeanalyzer) .</span><span class="sxs-lookup"><span data-stu-id="01c50-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="01c50-106">Bấm chuột phải vào **MDEClientAnalyzer. cmd** và chọn ' chạy với vai trò người quản trị '.</span><span class="sxs-lookup"><span data-stu-id="01c50-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="01c50-107">Làm theo bất kỳ hướng dẫn nào được đề xuất trong **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="01c50-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="01c50-108">Để biết thêm các Nhật ký tiết ra, hãy xem lại thư mục con đã tạo có tên là **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="01c50-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="01c50-109">Nếu cần có hướng dẫn bổ sung, hãy liên hệ với bộ [phận hỗ trợ của Microsoft cho điểm cuối](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) và cung cấp các tệp MDEClientAnalyzerResult.zip để phân tích.</span><span class="sxs-lookup"><span data-stu-id="01c50-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
