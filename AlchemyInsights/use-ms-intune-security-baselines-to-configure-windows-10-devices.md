---
title: Sử dụng cấu hình bảo mật của Microsoft InTune để cấu hình thiết bị chạy Windows 10
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
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573783"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Sử dụng cấu hình bảo mật của Microsoft InTune để cấu hình thiết bị chạy Windows 10

InTune bảo mật, giúp bảo vệ người dùng và thiết bị. Cấu hình bảo mật là các nhóm thiết đặt sẵn của Windows được dùng để áp dụng một nhóm thiết đặt đã biết và các giá trị mặc định được đề xuất bởi nhóm bảo mật liên quan. Bằng cách tạo hồ sơ đường cơ sở bảo mật trong InTune, bạn tạo một mẫu bao gồm nhiều hồ sơ cấu hình thiết bị.

Khi bạn triển khai các cấu hình bảo mật cho các nhóm người dùng hoặc thiết bị, các thiết đặt sẽ được áp dụng cho các thiết bị chạy trên Windows 10 trở lên. Ví dụ: MDM Security Baseline tự động (1) cho phép BitLocker cho ổ đĩa rời, (2) yêu cầu mật khẩu để mở khóa thiết bị và (3) vô hiệu hóa xác thực cơ bản. Khi một giá trị mặc định không hoạt động cho môi trường của bạn, hãy tùy chỉnh đường cơ sở để áp dụng các thiết đặt mà bạn cần.

Các đường căn bảo an cũng giúp thiết lập một dòng công việc bảo mật end-to-end trong Microsoft 365. Sau đây là một số lợi ích của việc này:

- Một đường cơ sở bảo mật bao gồm các biện pháp và đề xuất tốt nhất cho các thiết đặt ảnh hưởng đến bảo mật. Vì InTune đối tác với nhóm bảo mật Windows tạo ra các đường lưới cho các chính sách nhóm, các khuyến nghị này dựa trên hướng dẫn vững chắc và trải nghiệm rộng rãi.
- Nếu bạn mới dùng InTune và không chắc chắn bắt đầu từ đâu, sau đó sẽ giúp bạn nhanh chóng tạo và triển khai hồ sơ bảo mật.
- Nếu bạn hiện đang sử dụng chính sách nhóm, sau đó di chuyển đến InTune cho mục đích quản lý dễ dàng hơn nhiều so với các đường cơ bản, vì chúng được tích hợp vào InTune và bao gồm các khả năng cắt cạnh để quản lý.

Để tìm hiểu thêm, hãy xem các đường cơ sở [bảo mật của Windows](https://go.microsoft.com/fwlink/?linkid=2141503) và [quản lý thiết bị di động](https://go.microsoft.com/fwlink/?linkid=2141701).