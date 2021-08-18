---
title: Đặt cấu hình DLP Điểm cuối
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
ms.openlocfilehash: 97a8d4e7db9aac65e6a505c0bef8b41d2ea23353
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323940"
---
# <a name="configure-endpoint-dlp"></a>Đặt cấu hình DLP Điểm cuối

DLP Điểm cuối của Microsoft cho phép bạn mở rộng khả năng bảo vệ và giám sát DLP đối với thông tin nhạy cảm Windows 10 thiết bị. Sau khi thiết bị được triển lý vào quản lý thiết bị, bạn có thể tạo các chính sách DLP để thực thi các hành động bảo vệ trên các mục. Có thể dùng Activity Explorer để giám sát hoạt động cho các mục nhạy cảm. Để biết thêm thông tin, hãy xem [Mục Các thiết bị tích hợp vào quản lý thiết bị](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Để bắt đầu với DLP Điểm cuối:

- Ensure you have the appropriate SKU/subscriptions licensing. Để biết thêm thông tin, hãy [xem mục Cấp phép SKU/đăng ký.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)
- Kiểm tra các quyền cần thiết để cho phép quản lý thiết bị, truy nhập trang trình phát hoặc bật/tắt chức năng giám sát thiết bị. Để biết thêm thông tin, hãy [xem Quyền](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Đưa thiết bị vào Quản lý thiết bị bằng cách làm theo quy trình trên thiết bị. Để biết thêm thông tin, hãy [xem Mục Các thiết bị đang phát hành](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Tạo chính sách DLP để bảo vệ các mục nhạy cảm của bạn. Để biết thông tin, hãy [xem Các kịch bản chính sách DLP điểm cuối.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)

Để biết thêm thông tin về DLP Điểm cuối Microsoft, hãy xem Tìm hiểu về cách Microsoft 365 ngăn mất dữ liệu điểm cuối [(bản xem trước).](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about)

**Các bước Thu thập Dữ liệu Quan trọng nếu cần Hỗ trợ:**

1. Tải xuống [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).
1. Chạy công cụ với tư cách là Người quản trị từ cửa sổ cmd:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Khi được nhắc nhập số phút để thu thập dấu **vết:**, hãy nhập số phút cần thiết để chạy kịch bản.
1. Chạy kịch bản.

Thu thập đầu ra tệp Zip để tặng cho nhân viên Hỗ trợ.
