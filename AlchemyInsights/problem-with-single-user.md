---
title: Vấn đề với người dùng đơn lẻ
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
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430359"
---
# <a name="problem-with-single-user"></a>Vấn đề với người dùng đơn lẻ

- Người dùng có thể không được cung cấp bởi vì dịch vụ chưa có cơ hội đánh giá người dùng. Xem lại hướng dẫn về cách cung cấp dài mất, cũng như thanh tiến độ trên trang cấu hình cung cấp. Nếu trạng thái ổn định được xác định trong phần chi tiết bổ sung là trước ngày mà người dùng đã tạo/đã được Cập Nhật/đã xóa, điều đó có nghĩa là chúng tôi chưa đánh giá người dùng. Trong trường hợp này, điều tốt nhất cần làm là chờ cho dịch vụ cung cấp để kết thúc.

  - Lưu ý rằng dịch vụ của chúng tôi chỉ nhận thức được những thay đổi đối với người dùng trong hệ thống nguồn (đám mây nhân sự). Phải có thay đổi hợp lệ trong hệ thống nguồn cho Azure AD để phát hiện thay đổi và lưu nó thành Active Directory.
- Dịch vụ cung cấp sẽ đánh giá người dùng và xác định nó không nên được cung cấp:
  - Nếu bạn đã thiết lập bộ lọc dựa trên phạm vi thuộc tính, hãy đảm bảo rằng người dùng đáp ứng các tiêu chí mà bạn đã xác định.
  - Nếu người dùng đã tồn tại trong hệ thống đích và trạng thái của người dùng trong kết quả phù hợp với nguồn và đích, chúng tôi sẽ không thực hiện bất kỳ thao tác nào nữa.
- Dịch vụ cung cấp đã tìm cách cung cấp cho người dùng và không thành công. Đối với những tình huống này, hãy xem lại tab khắc phục sự cố và đề xuất của Nhật ký cung cấp:
  - Một thuộc tính bắt buộc trên người dùng có thể bị thiếu trong Active Directory tại chỗ hoặc Azure AD. Ví dụ, các quy tắc userPrincipalName hoặc sAMAccountName sẽ không tạo ra giá trị phù hợp.
  - Thuộc tính kết hợp (thường là employeeId) không giải quyết được một người dùng duy nhất trong Active Directory tại chỗ hoặc Azure AD. Ví dụ, có hai người dùng với cùng một employeeId trong quảng cáo và dịch vụ trả về một mã lỗi cho biết mục tiêu trùng lặp cho cùng một mục nhập nguồn.

Để xem lại Nhật ký dành cho người dùng và nhóm duy nhất, hãy xem [xem lại Nhật ký cung cấp cho vấn đề với một người dùng cụ thể](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).
