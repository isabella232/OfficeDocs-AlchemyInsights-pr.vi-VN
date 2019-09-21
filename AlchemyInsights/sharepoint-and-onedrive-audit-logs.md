---
title: Báo cáo Nhật ký kiểm tra SharePoint cổ điển
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068045"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Nhật ký kiểm tra SharePoint và OneDrive

**SharePoint và OneDrive hiện đại thống nhất kiểm tra Nhật ký từ tuân thủ**

- [Bật/tắt ghi nhật ký kiểm tra hợp nhất](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Không có cấu hình bổ sung được yêu cầu trong SharePoint hoặc OneDrive.

- Sử dụng kiểm tra ghi nhật ký tìm kiếm để kiểm tra hoạt động của tệp (s), cặp (s), người dùng (s), quyền:

    - [Hoạt động tập tin và trang](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [Hoạt động thư mục](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [Chia sẻ và truy cập các hoạt động yêu cầu](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [Hoạt động đồng bộ hóa](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [Hoạt động quản trị trang web](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- Để biết thêm thông tin về cách lấy các sự kiện, [hãy xem tìm kiếm Nhật ký kiểm tra](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).

**SharePoint cổ điển kiểm tra Nhật ký**

Chúng tôi đã di chuyển SPO kế thừa kiểm toán hợp nhất kiểm tra đăng nhập (UAL). Điều này về cơ bản có nghĩa là tất cả các báo cáo kiểm toán hợp lệ SPO bây giờ sẽ được cung cấp thông qua UAL, và các tín hiệu kiểm toán hợp lệ đã được di chuyển đến UAL.

Thay đổi chính:

- Trimming như là một khả năng không có sẵn.
- Phần mà bạn chọn các sự kiện cụ thể để kiểm tra là không có sẵn. Vui lòng tham khảo [tài liệu này](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) để biết danh sách đầy đủ các sự kiện được kiểm toán có sẵn theo mặc định.
- Tuỳ chọn "vị trí" trong **báo cáo tuỳ chỉnh** không khả dụng. 
- Sự kiện "mở hoặc tải xuống tài liệu" không khả dụng. 

