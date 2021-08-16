---
title: Đặt cấu hình dịch vụ Đồng bộ MIM
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
ms.openlocfilehash: f834bead0b6f22dcadc808d45dcefe7f6571ef62c74b7fd97355157ca49542af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978507"
---
# <a name="configure-mim-sync-service"></a>Đặt cấu hình dịch vụ Đồng bộ MIM

Dịch vụ Đồng bộ hóa Trình quản lý Định danh Microsoft (MIM) là một cấu phần của MIM. Đây là một dịch vụ tại cơ sở tập trung lưu trữ và tích hợp thông tin cho các tổ chức có nhiều thư mục và cơ sở dữ liệu tại cơ sở. Bạn có thể giải quyết sự cố của mình với MIM Sync nếu sự cố này được giải quyết trong bản cập nhật gần đây cho MIM hoặc là một trong các sự cố khác được đề cập trong mục bên dưới.

**Các bước được đề xuất**

1. Đảm bảo rằng bạn đang sử dụng bản cập nhật gần đây của MiM Sync và kiểm tra ghi chú phát hành [MiM Sync](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) để xác định xem sự cố đã được giải quyết trong bản cập nhật hay chưa.
2. Nếu sự cố xảy ra với bộ nối LDAP, Generic SQL, Lotus Domino hoặc Dịch vụ Web, hãy đảm bảo rằng bạn đang sử dụng bản cập nhật gần đây của các trình kết nối [chung.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)
3. Nếu chạy Đồng bộ MIM dừng với lỗi, hãy tham khảo bảng các mã lỗi chạy để xác định [các](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) nguyên nhân tiềm ẩn.
4. Nếu run stops with **extension-dll-exception,** then click on those words to open the **Connector Space Object** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).
5. Nếu cấu phần Dịch vụ Thông báo Thay đổi Mật khẩu (PCNS) báo cáo lỗi **6025** trong nhật ký sự kiện trong quá trình đồng bộ hóa mật khẩu, hãy xem hướng dẫn khắc phục sự cố lỗi báo cáo [PCNS 6025.](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)
6. Nếu quá trình đồng bộ hóa đầy đủ với  Tác vụ Quản lý Dịch vụ FIM chậm, hãy kiểm tra thiết đặt tự động phát triển cho TempDB, như được mô tả trong Khắc phục sự cố đồng bộ hóa chậm hoặc [treo.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)
7. Nếu bạn gặp phải lỗi của máy chủ đã dừng với dịch vụ tạo thông qua web không thành công bằng cách sử dụng Tác vụ Quản lý Dịch vụ FIM, hãy xem Hỗ [trợ-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) để biết tổng quan về các nguyên nhân.

