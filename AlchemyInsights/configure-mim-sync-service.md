---
title: Đặt cấu hình dịch vụ đồng bộ MIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482892"
---
# <a name="configure-mim-sync-service"></a>Đặt cấu hình dịch vụ đồng bộ MIM

Dịch vụ đồng bộ hóa Microsoft Identity Manager (MIM) là một thành phần của MIM. Đây là dịch vụ tại cơ sở tập trung lưu trữ và tích hợp thông tin cho các tổ chức có nhiều thư mục và cơ sở dữ liệu tại chỗ. Bạn có thể giải quyết vấn đề của mình với MIM đồng bộ nếu sự cố này đã được giải quyết trong bản cập nhật gần đây cho MIM hoặc là một trong các vấn đề khác được đề cập trong phần dưới đây.

**Các bước được đề xuất**

1. Đảm bảo rằng bạn đang sử dụng bản cập nhật gần đây về MIM đồng bộ và kiểm tra [ghi chú bản phát hành MIM Sync](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) để xác định xem vấn đề đã được giải quyết trong bản Cập Nhật hay không.
2. Nếu vấn đề là với LDAP chung, SQL chung chung, Lotus Domino hoặc trình kết nối dịch vụ web, hãy đảm bảo rằng bạn đang sử dụng bản cập nhật gần đây của các đường kết [nối chung](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).
3. Nếu điểm dừng đồng bộ chạy MIM với lỗi, hãy tham khảo bảng của các [mã lỗi chạy](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) để xác định các nguyên nhân tiềm ẩn.
4. Nếu các điểm dừng chạy với **phần mở rộng-dll-ngoại lệ**, sau đó bấm vào những từ này để mở cửa sổ **thuộc tính không gian kết nối** , rồi bấm vào theo **dõi stack...** để xem thêm thông tin về nguyên nhân cơ bản, như được mô tả trong [phần mở rộng-dll-ngoại lệ](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).
5. Nếu lỗi cấu phần dịch vụ thông báo thay đổi mật khẩu (PCNS), hãy chọn **6025** trong Nhật ký sự kiện khi đồng bộ hóa mật khẩu, đánh dấu phần hướng dẫn khắc phục sự cố [lỗi báo cáo PCNS 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).
6. Nếu việc đồng bộ hóa đầy đủ với tác nhân quản lý Dịch vụ FIM là chậm, hãy kiểm tra cài đặt **tự động phát triển** cho TempDB, như được mô tả trong [khắc phục sự cố chậm hoặc treo đồng bộ hóa đầy đủ](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).
7. Nếu bạn đang gặp phải lỗi dừng máy chủ với không thành công-qua-dịch vụ web bằng cách sử dụng tác nhân quản lý Dịch vụ FIM, hãy xem mục [hỗ trợ-thông tin: không thành công-thông qua-web-dịch vụ](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) để biết tổng quan về các nguyên nhân.

