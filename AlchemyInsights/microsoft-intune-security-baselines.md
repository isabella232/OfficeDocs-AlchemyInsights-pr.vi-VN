---
title: Sử dụng Microsoft Intune cơ sở bảo mật để đặt cấu hình cho các Windows 10 thiết bị
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 911c6b1860e4f44e6d88897f73173cdd11060562
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332007"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Sử dụng Microsoft Intune cơ sở bảo mật để đặt cấu hình cho các Windows 10 thiết bị

Đường cơ sở bảo mật intune giúp bảo vệ người dùng và thiết bị. Đường cơ sở bảo mật là Windows đặt sẵn được dùng để áp dụng một nhóm thiết đặt đã biết và các giá trị mặc định do các nhóm bảo mật liên quan đề xuất. Bằng cách tạo một hồ sơ đường cơ sở bảo mật trong Intune, bạn tạo một mẫu bao gồm nhiều hồ sơ cấu hình thiết bị.

Khi bạn triển khai đường cơ sở bảo mật cho các nhóm người dùng hoặc thiết bị, thiết đặt được áp dụng cho các thiết bị chạy trên Windows 10 hoặc mới hơn. Ví dụ: Đường cơ sở bảo mật quản lý thiết bị di động (MDM) của Microsoft tự động bật BitLocker cho ổ đĩa di động, yêu cầu mật khẩu để mở khóa thiết bị và tắt xác thực cơ bản. Khi một giá trị mặc định không hoạt động đối với môi trường của bạn, bạn có thể tùy chỉnh đường cơ sở để áp dụng các thiết đặt mà bạn cần.

Đường cơ sở bảo mật cũng giúp thiết lập một dòng công việc bảo mật đầu cuối trong Microsoft 365. Đường cơ sở bảo mật bao gồm các phương pháp và đề xuất tốt nhất cho các cài đặt ảnh hưởng đến bảo mật. Intune hợp tác với nhóm bảo mật Windows tạo đường cơ sở cho các chính sách nhóm, do đó, các đề xuất này dựa trên hướng dẫn đặc biệt và trải nghiệm chuyên sâu.

Nếu bạn mới sử dụng Intune và không chắc nên bắt đầu từ đâu, đường cơ sở bảo mật sẽ giúp bạn nhanh chóng tạo và triển khai hồ sơ bảo mật. Nếu bạn hiện đang sử dụng chính sách nhóm, việc di chuyển sang Intune cho mục đích quản lý sẽ dễ dàng hơn nhiều với đường cơ sở bảo mật vì chúng được tích hợp vào Intune và bao gồm các chức năng quản lý tiên tiến.

Để tìm hiểu thêm, hãy xem [Windows cơ sở bảo mật và Quản](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) lý thiết bị di [động](https://docs.microsoft.com/windows/client-management/mdm/).

