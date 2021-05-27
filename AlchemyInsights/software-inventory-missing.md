---
title: Kiểm kê phần mềm bị thiếu hoặc không chính xác
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676589"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>Kiểm kê phần mềm bị thiếu hoặc không chính xác

Kiểm kê phần mềm trong Quản lý Mối đe dọa và Lỗ hổng (TVM) là một danh sách phần mềm đã biết trong tổ chức của bạn với Công thức Liệt kê Nền tảng Chung (CPE) chính thức.

Sản phẩm phần mềm không có CPE chính thức không có lỗ hổng được phát hành. Hàng tồn kho cũng bao gồm các chi tiết như tên của nhà cung cấp, số lượng thiết bị tồn kho, mối đe dọa và số lượng thiết bị càng tiếp xúc.

Thay đổi phần mềm trên thiết bị thường được phản ánh trong cổng thông tin bảo mật trong vòng hai giờ. Tuy nhiên, đôi khi có thể mất nhiều thời gian hơn. Hiện không có cách nào để bắt buộc đồng bộ; đây là một đánh giá liên tục liên tục.

Nếu bạn thay đổi phần mềm và thay đổi không được phản ánh chính xác trong TVM sau 5 giờ, hãy làm theo các bước sau:

1. Kiểm tra phần bằng chứng phần mềm để tìm hiểu cách phần mềm được phát hiện.
1. Đảm bảo rằng phần mềm được hỗ trợ. Phần mềm có thể chỉ hiển thị ở cấp độ thiết bị ngay cả khi phần mềm hiện không được hỗ trợ Quản lý Mối đe dọa và Lỗ hổng. Tuy nhiên, chỉ có dữ liệu có giới hạn là khả dụng.
1. Để biết các bước báo cáo không chính xác từ cổng thông tin, hãy [xem Báo cáo không chính xác.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)
   
    **Lưu** ý : Báo cáo không chính xác từ cổng thông tin MDE là kênh một chiều cho đến kỹ thuật. Nếu sự cố này khẩn cấp, hãy mở thẻ hỗ trợ.

Để biết thêm thông tin, hãy [xem Kiểm kê phần mềm - Quản lý Mối đe dọa và Lỗ hổng.](/microsoft-365/security/defender-endpoint/tvm-software-inventory)