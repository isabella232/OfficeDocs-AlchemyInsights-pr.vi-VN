---
title: Sử dụng đường cơ sở Microsoft Intune quan để cấu hình các thiết Windows 10 khác nhau
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
ms.openlocfilehash: 3bb93c196dd4717f5ec297e63284c5bc2840dcf5965cd000f336fde1e982a061
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971541"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Sử dụng đường Microsoft Intune cơ sở bảo mật để đặt cấu hình cho thiết Windows 10 của bạn

Đường cơ sở bảo mật intune giúp bảo vệ người dùng và thiết bị. Đường cơ sở bảo mật là Windows cấu hình trước của thiết đặt, được dùng để áp dụng một nhóm thiết đặt đã biết và các giá trị mặc định do các nhóm bảo mật liên quan đề xuất. Bằng cách tạo hồ sơ đường cơ sở bảo mật trong Intune, bạn tạo một mẫu bao gồm nhiều hồ sơ cấu hình thiết bị.

Khi bạn triển khai đường cơ sở bảo mật cho các nhóm người dùng hoặc thiết bị, thiết đặt được áp dụng cho các thiết bị chạy trên Windows 10 bản mới hơn. Ví dụ: Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentications. Khi một giá trị mặc định không hoạt động đối với môi trường của bạn, bạn có thể tùy chỉnh đường cơ sở để áp dụng các thiết đặt mà bạn cần.

Đường cơ sở bảo mật cũng giúp thiết lập một dòng công việc bảo mật đầu cuối trong Microsoft 365. Sau đây là một số lợi ích của chức năng này:
- Đường cơ sở bảo mật bao gồm các phương pháp và đề xuất tốt nhất cho các cài đặt ảnh hưởng đến bảo mật. Vì Intune hợp tác với nhóm bảo mật Windows tạo đường cơ sở cho chính sách nhóm nên các đề xuất này dựa trên hướng dẫn đặc biệt và trải nghiệm chuyên sâu.
- Nếu bạn mới sử dụng Intune và không chắc nên bắt đầu từ đâu thì đường cơ sở bảo mật sẽ giúp bạn nhanh chóng tạo và triển khai hồ sơ bảo mật.
- Nếu bạn hiện đang sử dụng chính sách nhóm thì việc di chuyển sang Intune cho mục đích quản lý sẽ dễ dàng hơn nhiều với đường cơ sở bảo mật, vì các đường cơ sở bảo mật này được tích hợp vào Intune và bao gồm các chức năng tiên tiến để quản lý.

Để biết thêm thông tin, hãy [xem Windows cơ sở bảo mật và](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) Quản lý thiết bị di [động](https://docs.microsoft.com/windows/client-management/mdm/).