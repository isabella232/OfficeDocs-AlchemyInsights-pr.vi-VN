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
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a>Các vấn đề với máy triển khai vào Microsoft Defender cho các điểm cuối

Bạn có thể gặp sự cố với máy triển khai vào dịch vụ MDE. Nếu bạn có thể truy nhập vào máy người dùng cuối, hãy làm theo các bước sau:

1. Tải xuống phiên bản xem trước mới nhất của công cụ chẩn đoán [máy khách MDE](https://aka.ms/betamdeanalyzer) .
2. Bấm chuột phải vào **MDEClientAnalyzer. cmd** và chọn ' chạy với vai trò người quản trị '.
3. Làm theo bất kỳ hướng dẫn nào được đề xuất trong **MDEClientAnalyzer.htm**.
4. Để biết thêm các Nhật ký tiết ra, hãy xem lại thư mục con đã tạo có tên là **MDEClientAnalyzerResult**.
5. Nếu cần có hướng dẫn bổ sung, hãy liên hệ với bộ [phận hỗ trợ của Microsoft cho điểm cuối](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) và cung cấp các tệp MDEClientAnalyzerResult.zip để phân tích.
