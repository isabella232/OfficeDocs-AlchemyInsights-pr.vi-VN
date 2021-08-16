---
title: Di chuyển từ AIP sang NHÃN MIP/Hợp nhất trong Trung tâm Tuân thủ
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
ms.openlocfilehash: 378c3f58f77db8b23682432c942cd4f9c3a392651ca6564528a635724ad66a25
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000388"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Di chuyển từ AIP sang NHÃN MIP/Hợp nhất trong Trung tâm Tuân thủ

Để di chuyển từ nhãn AIP sang Nhãn Hợp nhất trong trung tâm Bảo mật và Tuân thủ, hãy làm như sau:

**Kích hoạt bảo vệ từ cổng thông tin Azure**

1. Nếu bạn chưa làm như vậy, hãy mở một cửa sổ trình duyệt mới [và đăng nhập vào cổng thông tin Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Dẫn hướng đến **azure Information Protection** blade. Ví dụ: trên menu hub, hãy bấm Tất **cả dịch vụ** và bắt đầu nhập **Thông** tin vào hộp Bộ lọc. Chọn **Azure Information Protection**. Nếu bạn chưa từng truy cập vào Azure Information Protection [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) blade trước đó, hãy xem các bước bổ sung một lần để thêm lưỡi này vào cổng thông tin. Để mở lưỡi Azure Information Protection, bạn phải có một gói đăng ký [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) hoặc một gói đăng Office 365 có bao gồm Rights Management. Nếu bạn có một trong những đăng ký này nhưng thấy thông báo rằng không tìm được đăng ký hợp lệ, hãy liên hệ với bộ phận Hỗ trợ của [Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) hoặc sử dụng các kênh hỗ trợ tiêu chuẩn của bạn.

2. Tìm tùy chọn menu **Quản** lý, rồi chọn Kích **hoạt bảo vệ**. Bấm vào **Kích hoạt**, rồi xác nhận hành động của bạn. Khi kích hoạt hoàn tất, thanh thông tin sẽ hiển thị Kích **hoạt thành công**.

**Di chuyển nhãn Azure Information Protection sang Trung Office 365 Tâm Bảo & Tuân thủ**

1. Đảm bảo rằng bạn đã đăng nhập với tư cách người dùng có quyền Người quản trị Toàn cầu.

2. Dẫn hướng đến **azure Information Protection** blade.

3. Từ tùy **chọn** menu Quản lý, hãy **chọn Nhãn hợp nhất**.

4. Trên Azure **Information Protection - Unified labeling** blade, bấm Activate và **làm** theo hướng dẫn trực tuyến.

**Lưu** ý : Xác minh rằng bạn có quyền thích hợp trước khi kích hoạt Di chuyển Trung tâm & tuân thủ Bảo mật. Xem các bài viết sau để biết thêm thông tin:

1. [Bạn cần là người quản trị toàn cầu để đặt cấu hình Azure Information Protection hay tôi có thể ủy nhiệm cho những người quản trị khác không?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Thông tin quan trọng về vai trò quản trị sau khi di chuyển sang Trung tâm & tuân thủ Bảo mật.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Để biết thêm thông tin về việc di chuyển AIP sang Nhãn Hợp nhất tới Trung tâm Bảo mật và Tuân thủ, hãy [xem Di chuyển nhãn.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)
