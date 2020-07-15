---
title: Vấn đề với máy bộ nhớ ngoài
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141840"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="0015a-102">Vấn đề với máy bộ nhớ ngoài</span><span class="sxs-lookup"><span data-stu-id="0015a-102">Issues with onboarding machines</span></span>

<span data-ttu-id="0015a-103">Bạn có thể gặp sự cố với máy in để dịch vụ MDATP.</span><span class="sxs-lookup"><span data-stu-id="0015a-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="0015a-104">Nếu bạn có thể truy cập vào máy người dùng cuối, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="0015a-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="0015a-105">Tải xuống công cụ chẩn đoán [máy khách kết nối phân tích](https://aka.ms/mdatpanalyzer) .</span><span class="sxs-lookup"><span data-stu-id="0015a-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="0015a-106">Giải nén và chạy MDATPAnalyzer. cmd.</span><span class="sxs-lookup"><span data-stu-id="0015a-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="0015a-107">Xác định vị trí Nhật ký chẩn đoán trong thư mục được gọi là MDATPClientAnalyzerResult, cùng một thư mục mà công cụ phân tích được tải xuống.</span><span class="sxs-lookup"><span data-stu-id="0015a-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="0015a-108">Đánh giá tệp nhật ký, MDATPClientAnalyzer.txt, để tìm sự cố kết nối hoặc cài đặt proxy Internet.</span><span class="sxs-lookup"><span data-stu-id="0015a-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>