---
title: Sự cố với người dùng đơn lẻ
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960173"
---
# <a name="problem-with-single-user"></a>Sự cố với người dùng đơn lẻ

- Có thể người dùng chưa được cung cấp vì dịch vụ chưa có cơ hội đánh giá người dùng. Xem lại hướng dẫn về khoảng thời gian cung cấp cũng như thanh tiến độ trên trang cấu hình cung cấp. Nếu trạng thái ổn định được chỉ định trong mục chi tiết bổ sung trước ngày người dùng được tạo/cập nhật/xóa, điều đó có nghĩa là chúng tôi chưa đánh giá người dùng. Trong kịch bản này, điều tốt nhất cần làm là chờ dịch vụ cung cấp kết thúc.

  - Lưu ý rằng dịch vụ của chúng tôi chỉ lưu ý tới các thay đổi đối với người dùng trong hệ thống nguồn (Cloud HR). Phải có một thay đổi hợp lệ trong hệ thống nguồn đối với Azure AD để phát hiện thay đổi và dòng dữ liệu đó vào Active Directory.
- Dịch vụ cung cấp đã đánh giá người dùng và xác định không nên cung cấp dịch vụ:
  - Nếu bạn đã đặt một bộ lọc phạm vi dựa trên thuộc tính, hãy đảm bảo rằng người dùng đáp ứng các tiêu chí mà bạn đã xác định.
  - Nếu người dùng đã tồn tại trong hệ thống đích và trạng thái của người dùng trong kết quả khớp nguồn và đích, chúng tôi sẽ không thực hiện thêm bất kỳ hành động nào.
- Việc cung cấp dịch vụ cố gắng cung cấp người dùng nhưng không thành công. Đối với các kịch bản này, hãy xem lại tab khắc phục sự cố và các đề xuất trong nhật ký cung cấp:
  - Thuộc tính bắt buộc của người dùng có thể bị thiếu trong Active Directory hoặc Azure AD tại chỗ. Ví dụ: quy tắc thế hệ userPrincipalName hoặc sAMAccountName không tạo giá trị phù hợp.
  - Thuộc tính khớp (thường là employeeId) không phân giải người dùng duy nhất trong Active Directory hoặc Azure AD tại chỗ. Ví dụ: có hai người dùng với cùng một nhân viênId trong AD và dịch vụ trả về mã lỗi cho biết mục nhập đích trùng lặp cho cùng một mục nhập nguồn.

Để xem lại nhật ký cho người dùng và nhóm đơn lẻ, hãy xem Xem lại [nhật ký cung cấp cho một sự cố với một người dùng cụ thể.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
