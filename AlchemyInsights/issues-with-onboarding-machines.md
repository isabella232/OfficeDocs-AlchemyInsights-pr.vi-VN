---
title: Các vấn đề với máy triển khai
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
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676904"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="7524e-102">Các vấn đề với máy triển khai</span><span class="sxs-lookup"><span data-stu-id="7524e-102">Issues with onboarding machines</span></span>

<span data-ttu-id="7524e-103">Bạn có thể gặp sự cố với máy triển khai vào dịch vụ mdatp.</span><span class="sxs-lookup"><span data-stu-id="7524e-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="7524e-104">Nếu bạn có thể truy nhập vào máy người dùng cuối, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="7524e-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="7524e-105">Tải xuống công cụ chẩn đoán [kết nối máy khách](https://aka.ms/mdatpanalyzer) .</span><span class="sxs-lookup"><span data-stu-id="7524e-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="7524e-106">Trích xuất và chạy MDATPAnalyzer. cmd.</span><span class="sxs-lookup"><span data-stu-id="7524e-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="7524e-107">Xác định vị trí Nhật ký chẩn đoán trong thư mục có tên là MDATPClientAnalyzerResult, cùng một thư mục mà công cụ phân tích được tải xuống.</span><span class="sxs-lookup"><span data-stu-id="7524e-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="7524e-108">Xem lại tệp nhật ký, MDATPClientAnalyzer.txt, để tìm các sự cố về kết nối hoặc thiết đặt proxy Internet.</span><span class="sxs-lookup"><span data-stu-id="7524e-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>