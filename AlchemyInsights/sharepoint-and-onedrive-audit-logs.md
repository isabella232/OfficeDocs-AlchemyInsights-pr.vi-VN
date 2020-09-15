---
title: Báo cáo Nhật ký kiểm tra SharePoint cổ điển
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662230"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Nhật ký kiểm tra SharePoint và OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Nhật ký kiểm tra cổ điển SharePoint

Mô hình thừa kế của SPO được di chuyển đến Nhật ký kiểm tra hợp nhất (UAL). Tất cả báo cáo kiểm nghiệm kế thừa của SPO sẽ được hỗ trợ thông qua UAL và các tín hiệu kiểm tra kế thừa đã được di chuyển đến UAL.

Các thay đổi then chốt:

* Dấu cắt không sẵn dùng như một khả năng.
* Chọn các sự kiện cụ thể để kiểm nghiệm không sẵn dùng. Tham khảo [tài liệu này](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) để biết danh sách đầy đủ các sự kiện được kiểm nhập sẵn dùng theo mặc định.
* Tùy chọn **vị trí** trong **báo cáo tùy chỉnh** không sẵn dùng.
* Tùy chọn **mở hoặc tải xuống** các sự kiện tài liệu không sẵn dùng.

[Cấu hình thiết đặt kiểm nghiệm cho tuyển tập trang](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Các Nhật ký kiểm tra hợp nhất trong SharePoint và OneDrive hiện đại từ việc tuân thủ

* [Bật/tắt ghi nhật ký kiểm tra hợp nhất](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

Không cần cấu hình bổ sung nào trong SharePoint hoặc OneDrive.

Sử dụng tính năng tìm kiếm Nhật ký kiểm tra để kiểm tra hoạt động của (các) tệp, (các) (các) (các) (các) người dùng, quyền:

* [Các hoạt động của tệp và trang](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Hoạt động của thư mục](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Các hoạt động yêu cầu chia sẻ và truy nhập](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Các hoạt động đồng bộ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Hoạt động quản trị site](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Để biết thêm thông tin về cách truy xuất các sự kiện này, hãy xem [Tìm kiếm Nhật ký kiểm](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)tra.
