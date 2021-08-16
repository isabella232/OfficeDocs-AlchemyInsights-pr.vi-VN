---
title: Công cụ xuất trong Khám phá Điện tử
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101324"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Bạn không thể cài đặt hoặc chạy Công cụ Xuất Khám phá Điện tử?

Nếu bạn không thể cài đặt hoặc chạy Công cụ Xuất Khám phá Điện tử để tải xuống kết quả tìm kiếm, hãy kiểm tra các mục sau:
  
- Máy tính bạn đang sử dụng cần đáp ứng các điều kiện tiên quyết sau:

  - Phiên bản 32 bit hoặc 64 bit từ Windows 7 trở lên

  - Microsoft .NET Framework 4.7.

  - Trình duyệt được hỗ trợ:

  - Microsoft Edge

    Hoặc

  - Internet Explorer 10 bản mới hơn

    Các trình duyệt khác, như Google Chrome và Mozilla Firefox không được hỗ trợ.

- Tổ chức của bạn có thể kết nối với điểm cuối trong Azure là **\* .blob.core.windows.net** (ký tự đại diện đại diện cho mã định danh duy nhất cho công việc xuất của bạn).

- Bạn được gán vai trò Xuất trong Trung tâm Tuân thủ Microsoft 365 &amp; Chính sách Bảo mật. Theo mặc định, vai trò này chỉ được gán cho nhóm có vai trò Người quản lý Khám phá Điện tử. Hãy [xem Gán các quyền Khám phá Điện tử.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Để biết thêm thông tin, hãy xem [Xuất kết quả Tìm kiếm Nội dung](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Nếu bạn đang xuất hơn 100K hộp thư, bạn sẽ cần sử dụng Powershell sau để tải xuống kết quả Xuất: Xuất kết quả từ  [hơn 100K hộp](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)thư.