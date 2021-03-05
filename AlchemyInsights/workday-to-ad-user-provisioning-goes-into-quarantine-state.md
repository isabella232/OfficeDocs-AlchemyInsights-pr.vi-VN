---
title: Ngày làm việc của người dùng quảng cáo đi sâu vào trạng thái cách ly
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
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482909"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Ngày làm việc của người dùng quảng cáo đi sâu vào trạng thái cách ly

**Ngày làm việc đến cấp phép người dùng quảng cáo đi sâu vào trạng thái kiểm soát và không người nào được tạo trong AD**

Ngày làm việc cho người dùng quảng cáo cung cấp công việc đã đi vào trạng thái cách ly và Nhật ký kiểm tra Hiển thị các sự kiện lỗi xuất hiện với lỗi thông báo lỗi **: OperationsError-SvcErr: một lỗi thao tác xảy ra. Không có tham chiếu vượt trội nào đã được cấu hình cho dịch vụ thư mục. Dịch vụ thư mục do đó không thể phát hiện các đối tượng được giới thiệu bên ngoài rừng này**. Lỗi này thường hiển thị nếu bộ chứa Active Directory OU không được đặt đúng hoặc nếu có vấn đề với ánh xạ biểu thức được sử dụng cho **Parentused Shedname**.

Chọn tham số OU mặc định cho **người dùng mới** cho lỗi chính tả. Đảm bảo rằng OU đã xác định đã tồn tại trong quảng cáo của bạn. Nếu bạn đang sử dụng **Parentscn shedname** trong ánh xạ thuộc tính, hãy đảm bảo rằng nó luôn được đánh giá là một bộ chứa đã biết trong tên miền quảng cáo. Kiểm tra sự kiện xuất trong Nhật ký kiểm nghiệm để xem giá trị được tạo ra.

Để biết thêm chi tiết về cách đặt cấu hình ngày làm việc cho tính năng cung cấp tự động, hãy xem [hướng dẫn: cấu hình ngày làm việc cho người dùng tự động cung](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)cấp.

