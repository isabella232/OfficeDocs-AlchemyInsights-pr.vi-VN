---
title: Di chuyển từ AIP đến MIP/ghi nhãn hợp nhất trong Trung tâm tuân thủ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825393"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Di chuyển từ AIP đến MIP/ghi nhãn hợp nhất trong Trung tâm tuân thủ

Để di chuyển từ nhãn AIP để ghi nhãn hợp nhất trong Trung tâm bảo mật và tuân thủ, hãy thực hiện như sau:

**Kích hoạt bảo vệ từ cổng thông tin Azure**

1. Nếu bạn chưa làm như vậy, hãy mở một cửa sổ trình duyệt mới và [đăng nhập vào cổng thông tin Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Dẫn hướng đến lưỡi dao **bảo vệ thông tin Azure** . Ví dụ, trên menu Hub, bấm vào **tất cả dịch vụ** và bắt đầu nhập **thông tin** trong hộp bộ lọc. Chọn **Azure Information Protection**. Nếu bạn chưa truy nhập vào lưỡi trước khi bảo vệ thông tin Azure, hãy xem các [bước bổ sung](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) một lần để thêm lưỡi dao này vào cổng thông tin. Để mở các lưỡi dao bảo vệ thông tin Azure, bạn phải có một [gói bảo vệ thông tin Azure](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) hoặc gói Office 365 bao gồm quản lý quyền. Nếu bạn có một trong các đăng ký này nhưng nhìn thấy thông báo rằng không tìm thấy một thuê bao hợp lệ, [hãy liên hệ với bộ phận](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) hỗ trợ của Microsoft hoặc dùng các kênh hỗ trợ tiêu chuẩn của bạn.

2. Xác định vị trí tùy chọn **quản lý** menu, rồi chọn **bảo vệ kích hoạt**. Bấm **kích hoạt**, rồi xác nhận hành động của bạn. Khi quá trình kích hoạt hoàn tất, thanh thông tin sẽ hiển thị việc **kích hoạt đã hoàn tất thành công**.

**Di chuyển nhãn bảo vệ thông tin Azure lên Trung tâm tuân thủ & bảo mật của Office 365**

1. Hãy đảm bảo bạn đã đăng nhập với tư cách người dùng với quyền của người quản trị toàn cầu.

2. Dẫn hướng đến lưỡi dao **bảo vệ thông tin Azure** .

3. Từ tùy chọn **quản lý** menu, chọn **ghi nhãn hợp nhất**.

4. Trên thanh **bảo vệ thông tin Azure-** lưỡi cắt dán hợp nhất, hãy bấm **kích hoạt** và làm theo hướng dẫn trực tuyến.

**Lưu ý**: xác nhận rằng bạn có quyền thích hợp trước khi kích hoạt di chuyển trung tâm tuân thủ & bảo mật. Xem các bài viết này để biết thêm thông tin:

1. [Bạn có cần phải là người quản trị toàn cầu để cấu hình bảo vệ thông tin Azure hoặc tôi có thể đại diện cho các người quản trị khác không?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Thông tin quan trọng về các vai trò quản trị sau khi di chuyển sang Trung tâm tuân thủ & bảo mật.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Để biết thêm thông tin về việc di chuyển nhãn hiệu của AIP để được thống nhất sang Trung tâm bảo mật và tuân thủ, hãy xem [di chuyển nhãn](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
