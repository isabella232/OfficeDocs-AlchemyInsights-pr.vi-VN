---
title: Di chuyển từ AIP sang MIP/ghi nhãn hợp nhất trong Trung tâm tuân thủ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7ce9c387fc94f59674a922c5fe071fc0fb030344
ms.sourcegitcommit: e6d73d240669342fde9d4d25b0ee2838b7e43965
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/14/2020
ms.locfileid: "44236563"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Di chuyển từ AIP sang MIP/ghi nhãn hợp nhất trong Trung tâm tuân thủ

Để di chuyển từ nhãn AIP sang ghi nhãn hợp nhất trong Trung tâm bảo mật và tuân thủ, hãy làm như sau:

**Kích hoạt bảo vệ từ cổng Azure**

1. Nếu bạn chưa làm như vậy, hãy mở cửa sổ trình duyệt mới và [đăng nhập vào cổng thông tin Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Điều hướng đến lưỡi **bảo vệ thông tin Azure** . Ví dụ: trên menu Trung tâm, bấm vào **tất cả các dịch vụ** và bắt đầu nhập **thông tin** trong hộp lọc. Chọn **bảo vệ thông tin Azure**. Nếu bạn chưa truy cập lưỡi bảo vệ thông tin Azure trước đó, hãy xem các [bước bổ sung](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) một lần để thêm lưỡi này vào cổng thông tin. Để mở lưỡi bảo vệ thông tin Azure, bạn phải có [gói Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) hoặc gói Office 365 bao gồm quản lý quyền. Nếu bạn có một trong các mục đăng ký nhưng thấy thông báo rằng đăng ký hợp lệ không thể tìm thấy, hãy [liên hệ với Microsoft support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) hoặc sử dụng kênh hỗ trợ tiêu chuẩn của bạn.

2. Tìm tùy chọn **quản lý** menu và chọn **kích hoạt bảo vệ**. Bấm **kích hoạt**, và sau đó xác nhận hành động của bạn. Khi kích hoạt hoàn tất, thanh thông tin hiển thị **kích hoạt hoàn tất thành công**.

**Di chuyển Azure bảo vệ thông tin nhãn cho Office 365 bảo mật & Trung tâm tuân thủ**

1. Đảm bảo rằng bạn đã đăng nhập người dùng với quyền quản trị toàn cầu.

2. Điều hướng đến lưỡi **bảo vệ thông tin Azure** .

3. Từ tùy chọn **quản lý** menu, chọn **ghi nhãn hợp nhất**.

4. Trên **Azure thông tin bảo vệ-hợp nhất nhãn** Blade, bấm **kích hoạt** và làm theo hướng dẫn trực tuyến.

**Lưu ý**: xác minh rằng bạn có quyền thích hợp trước khi kích hoạt di chuyển trung tâm tuân thủ & bảo mật. Xem các bài viết này để biết thêm thông tin:

1. [Bạn có cần phải là quản trị viên toàn cầu để cấu hình bảo vệ thông tin Azure hoặc tôi có thể ủy nhiệm cho các quản trị viên khác không?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Thông tin quan trọng về vai trò quản trị sau khi di chuyển sang bảo mật & tuân thủ trung tâm.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Để biết thêm thông tin về AIP để di chuyển ghi nhãn hợp nhất vào Trung tâm bảo mật và tuân thủ, hãy xem [di chuyển nhãn](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
