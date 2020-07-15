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
# <a name="issues-with-onboarding-machines"></a>Vấn đề với máy bộ nhớ ngoài

Bạn có thể gặp sự cố với máy in để dịch vụ MDATP. Nếu bạn có thể truy cập vào máy người dùng cuối, hãy làm theo các bước sau:

1. Tải xuống công cụ chẩn đoán [máy khách kết nối phân tích](https://aka.ms/mdatpanalyzer) .
2. Giải nén và chạy MDATPAnalyzer. cmd.
3. Xác định vị trí Nhật ký chẩn đoán trong thư mục được gọi là MDATPClientAnalyzerResult, cùng một thư mục mà công cụ phân tích được tải xuống.
4. Đánh giá tệp nhật ký, MDATPClientAnalyzer.txt, để tìm sự cố kết nối hoặc cài đặt proxy Internet.