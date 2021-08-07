---
title: Di chuyển thư mục công cộng không thành công ở 95%
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: e92a983a74ac0b97a613723dacb356ebff68f6cdba2d78ca63085a818d12e739
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923333"
---
# <a name="public-folder-migration-fails-at-95"></a>Di chuyển thư mục công cộng không thành công ở 95%

Bạn có thể đã bắt đầu hoàn tất một lô di chuyển và trạng thái của lô di chuyển sẽ tiếp tục hiển thị **Đã** đồng bộ trong một thời gian rất dài. Đây là hành vi được mong đợi.

Điều này thường gặp khi trạng thái  của một lô di chuyển vẫn được bật Đã đồng bộ trong một vài giờ trước khi nó chuyển **sang Hoàn thành**. Đối với các di chuyển liên quan đến số lượng lớn hộp thư đích, điều bình thường là thấy trạng thái vẫn ở trạng thái đã đồng bộ trong hơn 24 giờ, miễn là không có yêu cầu di chuyển thư mục công cộng cơ bản nào bị lỗi hoặc bị cách ly. Vui lòng cho phép lô di chuyển hoàn thành các nhiệm vụ trong 24-48 giờ.

Đối với việc di chuyển thư mục công cộng không thành công ở mức 95%, với lỗi FailedToMailEnablePublicFoldersException:

1. Tải xuống và chạy [tập lệnh ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) tại Exchange chủ Tại chỗ của bạn.

2. Thực hiện các hành động sửa được đề xuất bởi tập lệnh.

3. Chạy phiên bản Sync-MailPublicFolders (cho Exchange 2010) hoặc Sync-ModernMailPublicFolders (cho Exchange 2013 trở lên).

4. Tiếp tục di chuyển thư mục công cộng.
