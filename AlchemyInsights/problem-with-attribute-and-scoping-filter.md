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
ms.openlocfilehash: 51ed0fabe220d0069d721ec64d049787bacd5b094e19f0c1996a28e07bb56f03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960209"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Sự cố với bộ lọc thuộc tính và phạm vi

**Sự cố với các giá trị UPN xung đột**

The Workday to AD User Provisioning Workday to AD User Provisioning shows error **message HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**. Thao tác không thành công vì giá trị UPN được cung cấp để bổ sung/sửa đổi không phải là duy nhất trên toàn rừng. Chi tiết Lỗi: **CONSTRAINT_ATT_TYPE - userPrincipalName**.

Giá **trị userPrincipalName** mà bộ nối Workday đang cố gắng đặt khi tạo tài khoản người dùng AD đã tồn tại trong miền AD đích. Điều này ngụ ý rằng (1) người dùng đã tồn tại và kiểm tra ID khớp không thành công cho người dùng hoặc (2) quy tắc thế hệ UPN đã tạo ra một giá trị xung đột.

Dưới đây là các bước giải quyết được đề xuất:

Nếu người dùng đã tồn tại và kiểm tra ID khớp không thành công để liên kết tài khoản Ngày làm việc với tài khoản Active Directory, hãy kiểm tra xem liệu thuộc tính ID khớp **(thường** là ID nhân viên ) trong cả Ngày làm việc và AD có kết quả khớp chính xác hay không. Nếu không có trùng khớp thì đây là sự cố về dữ liệu cần được khắc phục. Ví dụ: nếuID Nhân viên trong Ngày làm việc là 001052 và trong AD đó là 1052 thì công cụ cung cấp sẽ không liên kết hai tài khoản này và sẽ cố gắng tạo một người dùng đã tồn tại. Giải pháp trong trường hợp này là thay đổi giá **trịID nhân** viên trong AD để đưa vào các số không đứng đầu để tạo giá trị 001052.
Nếu biểu thức UPN tạo ra không tạo ra một giá trị duy nhất, hãy cân nhắc sử dụng hàm de-duplication **SelectUniqueValue** để tạo một giá trị duy nhất mỗi lần.

**Ngày làm việc cho Cung cấp người dùng AD không đặt giá trị thuộc tính người quản lý cho tài khoản người dùng AD**

Công việc Ngày làm việc cho Người dùng Cung cấp AD không đặt giá trị thuộc **tính người quản** lý cho tài khoản người dùng AD. Có hai kịch bản có thể xảy ra khi hành vi này xuất hiện:

1. Không thể giải quyết người quản lý trong Ngày làm việc tới tài khoản Người dùng AD tương ứng vì người quản lý không nằm trong phạm vi.
2. Trong kịch **bản nhiều tên miền AD,** người quản lý trong Workday không hiện diện trong cùng một tên miền với người dùng.

Hãy thử các bước sau để giải quyết vấn đề này:

1. Nếu bạn đã xác định lọc phạm vi, trước tiên hãy kiểm tra xem người quản lý có nằm trong phạm vi không và bộ lọc đó có đáp ứng mệnh đề phạm vi không. Nếu người quản lý không đáp ứng bộ lọc phạm vi, hãy thay đổi bộ lọc để người quản lý cũng nằm trong phạm vi hoạt động cung cấp.
2. Nếu bạn có nhiều tên miền AD, thì bộ nối sẽ có giới hạn đã biết về không thể giải quyết các tham chiếu trình quản lý chéo miền.

Để biết thêm chi tiết về việc đặt cấu hình ngày làm việc cho việc cung cấp tự động, hãy xem mục Hướng dẫn: Đặt cấu hình Ngày làm việc [để cung cấp tự động cho người dùng.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)













