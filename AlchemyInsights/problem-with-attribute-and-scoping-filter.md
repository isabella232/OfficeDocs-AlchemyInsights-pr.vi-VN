---
title: Sự cố với bộ lọc thuộc tính và phạm vi
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
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482927"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Sự cố với bộ lọc thuộc tính và phạm vi

**Vấn đề với giá trị UPN xung đột**

Ngày làm việc cho người dùng quảng cáo cung cấp các ngày làm việc đến cấp phép người dùng quảng cáo hiển thị thông báo lỗi **Hybridsíp, Userprincipalnamenotunique**. Thao tác không thành công vì giá trị UPN được cung cấp cho việc bổ sung/sửa đổi không phải là duy nhất toàn rừng. Chi tiết lỗi: **CONSTRAINT_ATT_TYPE-userPrincipalName**.

Giá trị **userPrincipalName** mà đường kết nối ngày làm việc đang cố gắng đặt khi tạo tài khoản người dùng quảng cáo đã tồn tại trong tên miền quảng cáo đích. Điều này ngụ ý rằng một trong hai (1) người dùng đã tồn tại và ID kết hợp không thể kiểm tra được đối với người dùng hoặc (2) quy tắc thế hệ UPN tạo ra một giá trị xung đột.

Dưới đây là các bước giải quyết được đề xuất:

Nếu người dùng đã tồn tại và ID kết hợp sẽ không liên kết với tài khoản workday với tài khoản Active Directory, thì hãy kiểm tra xem liệu thuộc tính ID khớp (thường là **employeeID**) trong cả ngày làm việc và quảng cáo đều có kết quả khớp chính xác. Nếu họ không có kết quả khớp, đó là một vấn đề dữ liệu cần được khắc phục. Ví dụ, nếu EmployeeID trong ngày làm việc là 001052 và trong AD là 1052, thì công cụ cung cấp sẽ không liên kết hai tài khoản và sẽ cố gắng tạo một người dùng đã tồn tại. Giải pháp trong trường hợp này là để thay đổi giá trị **EmployeeID** trong AD để đưa vào số không đứng đầu để làm cho nó 001052.
Nếu biểu thức tạo UPN không tạo ra một giá trị duy nhất, hãy cân nhắc việc sử dụng hàm de-trùng lặp **SelectUniqueValue** để tạo một giá trị duy nhất mỗi lần.

**Ngày làm việc cho người dùng quảng cáo không đặt giá trị thuộc tính Manager cho tài khoản người dùng quảng cáo**

Ngày làm việc đến người dùng quảng cáo sẽ không đặt giá trị thuộc tính **Manager** cho tài khoản người dùng quảng cáo. Có hai tình huống có thể xảy ra khi hành vi này được nhìn thấy:

1. Trình quản lý trong ngày làm việc không thể được giải quyết cho tài khoản người dùng quảng cáo tương ứng vì người quản lý không nằm trong phạm vi.
2. Trong một kịch bản **nhiều tên miền quảng cáo** , trình quản lý trong ngày làm việc không có trong cùng tên miền với người dùng.

Hãy thử các bước sau để giải quyết vấn đề này:

1. Nếu bạn đã xác định bộ lọc có phạm vi, trước tiên, hãy kiểm tra xem người quản lý có được và điều đó thỏa mãn mệnh đề phạm vi hay không. Nếu người quản lý không thỏa mãn bộ lọc có phạm vi, hãy thay đổi bộ lọc để người quản lý đó cũng có thể sử dụng thao tác cung cấp.
2. Nếu bạn có nhiều tên miền quảng cáo, thì đường kết nối có giới hạn đã biết không có khả năng giải quyết tham chiếu trình quản lý miền chéo.

Để biết thêm chi tiết về cách đặt cấu hình ngày làm việc cho tính năng cung cấp tự động, hãy xem [hướng dẫn: cấu hình ngày làm việc cho người dùng tự động cung](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)cấp.













