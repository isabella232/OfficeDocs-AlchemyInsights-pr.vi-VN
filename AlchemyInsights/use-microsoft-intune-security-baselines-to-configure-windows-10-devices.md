---
title: Sử dụng trình nền bảo mật InTune của Microsoft để cấu hình thiết bị chạy Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696387"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Sử dụng trình nền bảo mật InTune của Microsoft để cấu hình các thiết bị chạy Windows 10

InTune bảo mật, giúp bảo vệ người dùng và thiết bị. Cấu hình bảo mật là các nhóm thiết đặt sẵn của Windows được dùng để áp dụng một nhóm thiết đặt đã biết và các giá trị mặc định được đề xuất bởi nhóm bảo mật liên quan. Bằng cách tạo hồ sơ đường cơ sở bảo mật trong InTune, bạn tạo một mẫu bao gồm nhiều hồ sơ cấu hình thiết bị.

Khi bạn triển khai các cấu hình bảo mật cho các nhóm người dùng hoặc thiết bị, các thiết đặt sẽ được áp dụng cho các thiết bị chạy trên Windows 10 hoặc các phiên bản mới hơn. Ví dụ: cơ sở tự động bảo mật quản lý thiết bị di động (MDM) của Microsoft (1) cho phép BitLocker cho ổ đĩa rời, (2) yêu cầu mật khẩu để mở khóa thiết bị và (3) vô hiệu hóa xác thực cơ bản. Khi một giá trị mặc định không hoạt động cho môi trường của bạn, bạn có thể tùy chỉnh đường cơ sở để áp dụng các thiết đặt mà bạn cần.

Các đường căn bảo an cũng giúp thiết lập một dòng công việc bảo mật end-to-end trong Microsoft 365. Sau đây là một số lợi ích của chức năng này:
- Một đường cơ sở bảo mật bao gồm các biện pháp và đề xuất tốt nhất cho các thiết đặt ảnh hưởng đến bảo mật. Vì InTune đối tác với nhóm bảo mật Windows tạo ra các đường lưới cho các chính sách nhóm, các khuyến nghị này dựa trên hướng dẫn vững chắc và trải nghiệm rộng rãi.
- Nếu bạn mới dùng InTune và không chắc chắn bắt đầu từ đâu, sau đó sẽ giúp bạn nhanh chóng tạo và triển khai hồ sơ bảo mật.
- Nếu bạn hiện đang sử dụng chính sách nhóm, sau đó di chuyển đến InTune cho các mục đích quản lý sẽ dễ dàng hơn nhiều so với các đường kết hợp bảo mật, bởi vì các đường cơ sở bảo mật này được tích hợp vào InTune và bao gồm các khả năng cắt cạnh để quản lý.

Để biết thêm thông tin, hãy xem bộ [phận bảo mật của Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) và [quản lý thiết bị di động](https://docs.microsoft.com/windows/client-management/mdm/).