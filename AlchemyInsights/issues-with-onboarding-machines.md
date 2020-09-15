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
# <a name="issues-with-onboarding-machines"></a>Các vấn đề với máy triển khai

Bạn có thể gặp sự cố với máy triển khai vào dịch vụ mdatp. Nếu bạn có thể truy nhập vào máy người dùng cuối, hãy làm theo các bước sau:

1. Tải xuống công cụ chẩn đoán [kết nối máy khách](https://aka.ms/mdatpanalyzer) .
2. Trích xuất và chạy MDATPAnalyzer. cmd.
3. Xác định vị trí Nhật ký chẩn đoán trong thư mục có tên là MDATPClientAnalyzerResult, cùng một thư mục mà công cụ phân tích được tải xuống.
4. Xem lại tệp nhật ký, MDATPClientAnalyzer.txt, để tìm các sự cố về kết nối hoặc thiết đặt proxy Internet.