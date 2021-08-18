---
title: Các chỉ báo không hoạt động khi sử dụng trình duyệt Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: 2a48a49ec52a585e450edf448bc9203cd9c3f935
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326283"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Các chỉ báo không hoạt động khi sử dụng trình duyệt Edge

Sau khi bạn đã tạo Một Chỉ báo, Edge (Màn hình thông minh) không có chức năng này. Để biết thêm thông tin, [hãy xem Tạo chỉ báo cho CÁC URL và URL/miền.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>Bước 1: Đảm bảo các bước sau

- Xác minh rằng chỉ báo là chính xác (không có lỗi đánh máy trong IP/URL, sửa hành động, nhóm RBAC chính xác).
- Hãy chờ tối thiểu 2 giờ sau khi tạo chỉ báo để tính đến độ trễ có thể xảy ra.
- Xác nhận rằng (các) hệ thống được tích hợp vào Bộ bảo vệ Microsoft dành cho Điểm cuối.
- Xác minh (các) hệ thống có thể liên lạc với Đám mây.
- Xác minh rằng Smartscreen đã được bật và có thể tiếp cận bằng cách đi tới [site thử nghiệm](https://demo.smartscreen.msft.net).

## <a name="step-2-troubleshoot-the-potential-issue"></a>Bước 2: Khắc phục sự cố tiềm ẩn

- Hãy đảm bảo máy khách đáp ứng các yêu cầu. Để biết chi tiết, [hãy xem Tạo chỉ báo cho CÁC URL và URL/tên miền](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain).
- Đảm bảo rằng bạn đang chạy phiên bản trình duyệt Edge mới nhất. Để tìm hiểu phiên bản mới nhất, hãy [xem Tìm hiểu xem bạn có phiên bản Microsoft Edge nào.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- Khởi động lại trình duyệt Edge.
- Dẫn hướng đến site mà bạn đã thiết lập một chỉ báo. Nếu site không xuất hiện như mong đợi, hãy tiếp tục đến Bước 3. 

## <a name="step-3-collect-data"></a>Bước 3: Thu thập dữ liệu

- Thu **thập dữ liệu chẩn đoán MDEClientAnalyzer.** Để biết hướng dẫn, hãy [xem mục Các sự cố với máy tiếp thị đối với Microsoft Defender dành cho Điểm cuối.](issues-with-onboarding-machines.md)
- Nếu bạn cảm thấy thoải mái khi cài đặt và thu thập dấu vết Fiddler, hãy xem [Telerik Fiddler.](http://www.telerik.com/fiddler)
- Nếu bạn muốn xem hướng dẫn từ Bộ hỗ trợ của Microsoft, hãy chọn biểu tượng Hỗ trợ bên dưới để mở trường hợp hỗ trợ.
