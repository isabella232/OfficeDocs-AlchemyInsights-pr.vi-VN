---
title: Cung cấp cho người dùng
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
- "9004348"
- "8428"
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971361"
---
# <a name="user-provisioning"></a>Cung cấp cho người dùng

- Sử dụng chức [năng cung cấp theo yêu cầu](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) để cung cấp người dùng và nhận được chẩn đoán chi tiết về các bước thực hiện.
- Để khắc phục sự cố bạn gặp phải khi cung cấp người dùng và nhóm, hãy xem hướng dẫn khắc phục sự [cố Không người dùng nào đang được cung cấp.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Nếu bạn thấy người dùng không được cung cấp, hãy xem mục Cung cấp nhật ký [(xem trước)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) trong Azure Active Directory (AD). Tìm kiếm các mục nhật ký liên quan đến một người dùng cụ thể.
- Hãy khởi động lại việc cung cấp định kỳ để nắm bắt bất kỳ người dùng nào đã bỏ lỡ trong chu kỳ cung cấp trước đó.
- Người dùng/nhóm có thể chưa được cung cấp vì dịch vụ của chúng tôi chưa có cơ hội đánh giá người dùng. Xem lại hướng dẫn về khoảng thời gian cung cấp cũng như thanh tiến độ trên trang cấu hình cung cấp. Nếu trạng thái ổn định được chỉ định trong mục chi tiết bổ sung trước ngày người dùng được tạo/cập nhật/xóa, điều đó có nghĩa là chúng tôi chưa đánh giá người dùng. Trong kịch bản này, điều tốt nhất cần làm là chờ dịch vụ cung cấp kết thúc. Nếu đạt được trạng thái ổn định, chúng tôi khuyên bạn nên thực hiện khởi động lại từ UI trong Cổng thông tin Azure.
  - Lưu ý rằng dịch vụ của chúng tôi chỉ biết về những thay đổi đối với người dùng/nhóm trong hệ thống nguồn (Azure Active Directory). Nếu người dùng/nhóm bị loại bỏ trực tiếp trong ứng dụng (ví dụ: ServiceNow), chúng tôi không biết về những thay đổi đó và không quay số ra dựa trên trạng thái của người dùng trong hệ thống nguồn. Trong tình huống này, tốt nhất là nên quay trở lại thay đổi trực tiếp trong ứng dụng đích.
- Dịch vụ của chúng tôi đã đánh giá người dùng/nhóm và xác định không nên cung cấp dịch vụ:
  - Nếu bạn đã đặt phạm vi cho người dùng và nhóm được gán, hãy kiểm tra xem người dùng/nhóm có được gán cho ứng dụng hay không.
  - Nếu người dùng/nhóm được gán cho ứng dụng, hãy đảm bảo rằng họ không được gán vai trò truy nhập mặc định. Không thể sử dụng vai trò này để cung cấp.
  - Nếu bạn đã đặt một bộ lọc phạm vi dựa trên thuộc tính, hãy đảm bảo rằng người dùng đáp ứng các tiêu chí mà bạn đã xác định.
  - Nếu người dùng đã tồn tại trong hệ thống đích và trạng thái của người dùng trong kết quả khớp nguồn và đích, chúng tôi sẽ không thực hiện thêm bất kỳ hành động nào.
- Dịch vụ của chúng tôi đã cố gắng cung cấp cho người dùng nhưng không thành công. Đối với các kịch bản này, hãy xem lại tab khắc phục sự cố và các đề xuất trong nhật ký cung cấp:
  - Một thuộc tính bắt buộc của người dùng có thể bị thiếu trong Azure Active Directory hoặc không khớp với định dạng mà ứng dụng của bên thứ ba yêu cầu. Ví dụ, thuộc tính Quốc gia trên người dùng có thể được đặt là Hoa Kỳ khi thuộc tính này nên là Hoa Kỳ.
  - Thuộc tính là một thuộc tính tham chiếu chưa tồn tại trong ứng dụng đích. Thuộc tính tham chiếu là một thuộc tính chỉ tới một đối tượng khác, ví dụ: người dùng là thành viên của nhóm. ID của người dùng sẽ có trong thuộc tính thành viên của nhóm, nhưng chỉ có thể được xử lý nếu đối tượng người dùng đó chỉ đến đã tồn tại.
