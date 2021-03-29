---
title: Cấu hình điểm cuối
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402467"
---
# <a name="configure-endpoint-dlp"></a>Cấu hình điểm cuối

Microsoft điểm cuối cho phép bạn mở rộng khả năng bảo vệ và giám sát cho các thông tin nhạy cảm trên các thiết bị chạy Windows 10. Sau khi thiết bị được onchéo vào quản lý thiết bị, bạn có thể tạo chính sách có quy định thực thi hành động bảo vệ trên các mục. Có thể sử dụng trình khám phá hoạt động để theo dõi hoạt động cho các mục nhạy cảm. Để biết thêm thông tin, hãy xem [thiết bị Onboarding vào quản lý thiết bị](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Để bắt đầu với điểm cuối:

- Đảm bảo bạn có các mã bản quyền/gói đăng ký phù hợp. Để biết thêm thông tin, hãy xem [Mã sản phẩm/gói đăng ký](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Kiểm tra các quyền cần thiết để cho phép quản lý thiết bị, truy nhập trang triển khai hoặc bật/tắt giám sát thiết bị. Để biết thêm thông tin, hãy xem [quyền](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Thiết bị onboard vào quản lý thiết bị bằng cách làm theo quy trình thiết bị triển khai. Nếu bạn bị thiếu tùy chọn cài đặt Onboarding (bản xem trước) bên dưới  **thiết đặt** tuân thủ M365, hãy xác nhận bạn có giấy phép và quyền thích hợp được tham chiếu ở trên. Để biết thêm thông tin, hãy xem [thiết bị Onboarding](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Tạo chính sách có thể bảo vệ các mục nhạy cảm của bạn. Để biết thông tin, hãy xem các [kịch bản chính sách điểm cuối](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

Để biết thêm thông tin về Microsoft điểm cuối, hãy xem [Tìm hiểu về ngăn chặn mất dữ liệu về microsoft 365 Endpoint (bản xem trước)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Các bước thu thập dữ liệu quan trọng, nếu cần hỗ trợ:**

1. Tải xuống bản xem trước phân tích máy khách MDATP từ [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. Chạy công cụ dưới dạng quản trị từ cửa sổ CMD:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd – t
4. Khi được nhắc với "nhập số phút để thu thập các dấu vết:", hãy nhập số phút cần thiết để chạy kịch bản
5. Chạy kịch bản

Thu thập các đầu ra tệp ZIP để được cung cấp cho nhân viên hỗ trợ.
