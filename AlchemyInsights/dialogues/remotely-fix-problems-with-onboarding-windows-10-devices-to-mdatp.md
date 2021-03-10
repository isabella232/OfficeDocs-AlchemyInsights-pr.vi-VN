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
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Khắc phục sự cố từ xa với các thiết bị chạy Windows 10 cho bộ bảo vệ mối đe dọa nâng cao của Microsoft Defender

Nếu bạn có thể truy nhập vào máy tính từ xa, hãy làm theo các bước sau đây:

1. Tải xuống công cụ chẩn đoán [kết nối máy khách](https://go.microsoft.com/fwlink/?linkid=2143466) .
2. Trích xuất và chạy MDATPAnalyzer. cmd.
3. Xác định vị trí Nhật ký chẩn đoán trong thư mục MDATPClientAnalyzerResult, chính là thư mục mà công cụ phân tích đã được tải xuống.
4. Để tìm các vấn đề với kết nối hoặc thiết đặt proxy Internet, hãy xem lại MDATPClientAnalyzer.txt tệp nhật ký.

Để tìm hiểu thêm, hãy xem các [vấn đề với máy triển khai](https://go.microsoft.com/fwlink/?linkid=2143634).
