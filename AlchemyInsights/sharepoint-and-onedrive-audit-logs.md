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
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992640"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Nhật ký kiểm tra SharePoint và OneDrive

## <a name="sharepoint-classic-audit-logs"></a>SharePoint cổ điển kiểm tra Nhật ký

Kiểm tra kế thừa SPO được di chuyển sang Nhật ký kiểm tra hợp nhất (UAL). Tất cả các báo cáo kiểm toán kế thừa SPO sẽ được cung cấp thông qua UAL, và các tín hiệu kiểm toán hợp lệ đã được di chuyển đến UAL.

Thay đổi chính:

* Trimming là không có sẵn như là một khả năng.
* Chọn các sự kiện cụ thể để kiểm tra không có sẵn. Tham khảo [tài liệu này](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) để biết danh sách đầy đủ các sự kiện được kiểm toán có sẵn theo mặc định.
* Tùy chọn **vị trí** trong **báo cáo tùy chỉnh** không có sẵn.
* Tùy chọn **mở hoặc tải xuống** các sự kiện tài liệu không khả dụng.

[Cấu hình thiết đặt kiểm tra cho bộ sưu tập trang web](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint và OneDrive hiện đại thống nhất kiểm tra Nhật ký từ tuân thủ

* [Bật/tắt ghi nhật ký kiểm tra hợp nhất](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Không có cấu hình bổ sung được yêu cầu trong SharePoint hoặc OneDrive.

Sử dụng kiểm tra ghi nhật ký tìm kiếm để kiểm tra hoạt động của tệp (s), cặp (s), người dùng (s), quyền:

* [Hoạt động tập tin và trang](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Hoạt động thư mục](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Chia sẻ và truy cập các hoạt động yêu cầu](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Hoạt động đồng bộ hóa](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Hoạt động quản trị trang web](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Để biết thêm thông tin về cách lấy các sự kiện, [hãy xem tìm kiếm Nhật ký kiểm tra](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
