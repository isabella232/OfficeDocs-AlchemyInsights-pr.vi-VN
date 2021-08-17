---
title: Sử dụng Microsoft Intune cơ sở bảo mật để đặt cấu hình cho các Windows 10 thiết bị
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104366"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Sử dụng Microsoft Intune cơ sở bảo mật để đặt cấu hình cho các Windows 10 thiết bị

Đường cơ sở bảo mật intune giúp bảo vệ người dùng và thiết bị. Đường cơ sở bảo mật là Windows cấu hình trước của thiết đặt, được dùng để áp dụng một nhóm thiết đặt đã biết và các giá trị mặc định do các nhóm bảo mật liên quan đề xuất. Bằng cách tạo hồ sơ đường cơ sở bảo mật trong Intune, bạn tạo một mẫu bao gồm nhiều hồ sơ cấu hình thiết bị.

Khi bạn triển khai đường cơ sở bảo mật cho các nhóm người dùng hoặc thiết bị, thiết đặt được áp dụng cho các thiết bị chạy trên Windows 10 trở lên. Ví dụ: Đường cơ sở Bảo mật MDM tự động (1) bật BitLocker cho ổ đĩa di động, (2) yêu cầu mật khẩu để mở khóa thiết bị và (3) tắt xác thực cơ bản. Khi một giá trị mặc định không hoạt động đối với môi trường của bạn, hãy tùy chỉnh đường cơ sở để áp dụng các thiết đặt mà bạn cần.

Đường cơ sở bảo mật cũng giúp thiết lập một dòng công việc bảo mật đầu cuối trong Microsoft 365. Sau đây là một số lợi ích của việc này:

- Đường cơ sở bảo mật bao gồm các phương pháp và đề xuất tốt nhất cho các cài đặt ảnh hưởng đến bảo mật. Vì Intune hợp tác với nhóm bảo mật Windows tạo đường cơ sở cho chính sách nhóm nên các đề xuất này dựa trên hướng dẫn đặc biệt và trải nghiệm chuyên sâu.
- Nếu bạn mới sử dụng Intune và không chắc nên bắt đầu từ đâu thì đường cơ sở bảo mật sẽ giúp bạn nhanh chóng tạo và triển khai hồ sơ bảo mật.
- Nếu bạn hiện đang sử dụng chính sách nhóm thì việc di chuyển sang Intune cho mục đích quản lý sẽ dễ dàng hơn nhiều với đường cơ sở bảo mật, vì chúng được tích hợp sẵn trong Intune và bao gồm các chức năng tiên tiến để quản lý.

Để tìm hiểu thêm, hãy xem [Windows cơ sở bảo mật và](https://go.microsoft.com/fwlink/?linkid=2141503) Quản lý thiết bị di [động](https://go.microsoft.com/fwlink/?linkid=2141701).