---
title: Ngày làm việc cho Người dùng Cung cấp AD chuyển sang trạng thái cách ly
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
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036514"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Ngày làm việc cho Người dùng Cung cấp AD chuyển sang trạng thái cách ly

**Ngày làm việc cho Cung cấp Người dùng AD chuyển sang trạng thái cách ly và không có người dùng nào được tạo ra trong AD**

Công việc Ngày làm việc cho Người dùng Cung cấp AD đã chuyển sang trạng thái cách ly và nhật ký kiểm tra hiển thị các sự kiện xuất không thành công kèm theo thông báo lỗi **Lỗi: OperationsError-SvcErr: Đã xảy ra lỗi thao tác. Không có tham chiếu cao cấp nào được cấu hình cho dịch vụ thư mục. Do đó, dịch vụ thư mục không thể cấp thông báo giới thiệu đến các đối tượng bên ngoài rừng này.** Lỗi này thường xuất hiện nếu OU Bộ chứa Active Directory không được đặt chính xác hoặc nếu có sự cố với Ánh xạ Biểu thức được sử dụng cho **parentDistinguishedName.**

Kiểm tra tham số OU mặc **định cho Người dùng** Mới đối với lỗi đánh máy. Đảm bảo rằng OU được chỉ định đã tồn tại trong AD của bạn. Nếu bạn đang sử **dụng parentDistinguishedName** trong ánh xạ thuộc tính, hãy đảm bảo rằng nó luôn đánh giá cho bộ chứa đã biết trong tên miền AD. Kiểm tra sự kiện Export trong nhật ký kiểm tra để xem giá trị được tạo.

Để biết thêm chi tiết về việc đặt cấu hình ngày làm việc cho việc cung cấp tự động, hãy xem mục Hướng dẫn: Đặt cấu hình Ngày làm việc [để cung cấp tự động cho người dùng.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

