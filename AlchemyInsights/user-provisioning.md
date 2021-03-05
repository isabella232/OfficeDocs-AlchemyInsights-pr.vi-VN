---
title: Cung cấp người dùng
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
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482910"
---
# <a name="user-provisioning"></a>Cung cấp người dùng

- Sử dụng khả năng cung cấp theo [yêu cầu](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) để cung cấp cho người dùng và nhận chẩn đoán chi tiết về các bước được thực hiện.
- Để khắc phục sự cố mà bạn gặp phải khi cung cấp cho người dùng và nhóm, hãy xem hướng dẫn khắc phục sự cố khi [người dùng không được](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)cung cấp.
- Nếu bạn quan sát rằng người dùng không được cung cấp, hãy xem [Nhật ký cấp phép (bản xem trước)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) trong Azure Active Directory (quảng cáo). Tìm kiếm các mục nhập Nhật ký liên quan đến một người dùng cụ thể.
- Quyền khởi động lại định kỳ để bắt bất kỳ người dùng nào bị nhỡ trong vòng tròn cung cấp trước đó.
- Người dùng/nhóm có thể không được cung cấp bởi vì dịch vụ của chúng tôi chưa có cơ hội đánh giá người dùng. Xem lại hướng dẫn về cách cung cấp dài mất, cũng như thanh tiến độ trên trang cấu hình cung cấp. Nếu trạng thái ổn định được xác định trong phần chi tiết bổ sung là trước ngày mà người dùng đã tạo/đã được Cập Nhật/đã xóa, điều đó có nghĩa là chúng tôi chưa đánh giá người dùng. Trong trường hợp này, điều tốt nhất cần làm là chờ cho dịch vụ cung cấp để kết thúc. Nếu trạng thái ổn định đã đạt được, chúng tôi khuyên bạn nên thực hiện một khởi động lại từ UI trong cổng thông tin Azure.
  - Lưu ý rằng dịch vụ của chúng tôi chỉ nhận thức được những thay đổi đối với người dùng/nhóm trong hệ thống nguồn (Azure Active Directory). Nếu một người dùng/nhóm được loại bỏ trực tiếp trong ứng dụng (ví dụ, ServiceNow), chúng tôi không biết những thay đổi này và không cuộn nó trở lại dựa trên trạng thái của người dùng trong hệ thống nguồn. Trong trường hợp này, cách tốt nhất là cuộn ngược lại thay đổi trực tiếp trong ứng dụng đích.
- Dịch vụ của chúng tôi sẽ đánh giá người dùng/nhóm và xác định nó không nên được cung cấp:
  - Nếu bạn đã thiết lập phạm vi cho người dùng và nhóm, hãy kiểm tra xem liệu người dùng/nhóm được gán cho ứng dụng hay không.
  - Nếu người dùng/nhóm được gán cho ứng dụng, hãy đảm bảo rằng chúng không được gán cho vai trò truy nhập mặc định. Không thể sử dụng vai trò này để cung cấp.
  - Nếu bạn đã thiết lập bộ lọc dựa trên phạm vi thuộc tính, hãy đảm bảo rằng người dùng đáp ứng các tiêu chí mà bạn đã xác định.
  - Nếu người dùng đã tồn tại trong hệ thống đích và trạng thái của người dùng trong kết quả phù hợp với nguồn và đích, chúng tôi sẽ không thực hiện bất kỳ thao tác nào nữa.
- Dịch vụ của chúng tôi đã tìm cách cung cấp cho người dùng và không thành công. Đối với những tình huống này, hãy xem lại tab khắc phục sự cố và đề xuất của Nhật ký cung cấp:
  - Một thuộc tính bắt buộc trên người dùng có thể bị thiếu trong Azure Active Directory hoặc không khớp với định dạng được yêu cầu bởi ứng dụng của bên thứ ba. Ví dụ, thuộc tính quốc gia trên một người dùng có thể được đặt thành Hoa Kỳ khi chúng tôi phải là chúng tôi.
  - Thuộc tính là thuộc tính tham khảo vẫn chưa tồn tại trong ứng dụng đích. Thuộc tính tham hiệu là một thuộc tính trỏ tới một đối tượng khác, ví dụ: một người dùng là một thành viên của nhóm. ID của người dùng sẽ nằm trong thuộc tính thành viên của nhóm, nhưng chỉ có thể xử lý nếu đối tượng người dùng đó đã tồn tại.
