---
title: Sự cố khi đặt lại mật khẩu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039988"
---
# <a name="problems-resetting-password"></a>Sự cố đặt lại mật khẩu

Sau đây là một số sự cố mà bạn có thể gặp phải khi đặt lại mật khẩu và các giải pháp khả thi:

**Tôi đang gặp sự cố với việc đặt lại mật khẩu không được đề cập trong các danh mục khác**

- Đảm bảo bạn được phép đặt lại mật khẩu. Chỉ người quản trị toàn cục, mật khẩu và người dùng mới có thể đặt lại mật khẩu người dùng. Người quản trị toàn cầu cũng có thể đặt lại mật khẩu của người quản trị có đặc quyền khác.
- Đảm bảo rằng bạn hiểu các yêu cầu cấp phép:
    - Bạn phải có ít nhất một giấy phép được gán trong tổ chức của mình
        - Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic
        - Người dùng đám mây và/hoặc người dùng tại chỗ - Azure AD Premium P1 hoặc P2, Enterprise Mobility + Security (EMS) hoặc Azure SECURE PRODUCTIVE ENTERPRISE (SPE)
        - Để đọc thêm về yêu cầu cấp phép, hãy xem bài viết Yêu cầu cấp phép cho đặt lại [mật khẩu tự phục vụ Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tôi đang gặp sự cố khi kiểm tra chính sách đặt lại mật khẩu mà tôi đã đặt**

- Các chính sách được áp dụng gần đây có thể mất vài phút để sao chép trên tất cả các trung tâm dữ liệu và điểm cuối. Khoảng cách vật lý từ trung tâm dữ liệu cũng sẽ ảnh hưởng đến mức độ nhanh chóng thay đổi được áp dụng.
- Thử nghiệm với một người dùng cuối, không phải người quản trị, và thử nghiệm với một tập hợp nhỏ người dùng. Các chính sách được đặt cấu hình trong cổng thông tin Azure CHỈ áp dụng cho người dùng cuối, không áp dụng cho người quản trị. Microsoft sẽ bắt buộc chính sách đặt lại mật khẩu hai cổng mặc định mạnh cho mọi vai trò người quản trị Azure (Ví dụ: Người quản trị Toàn cầu, Người quản trị Bộ trợ giúp, Người quản trị Mật khẩu, v.v.)
    - Tìm hiểu thêm về [các chính sách dành cho người quản trị.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Tôi muốn triển khai đặt lại mật khẩu nhưng tôi không muốn người dùng của mình đăng ký thông tin bảo mật bổ sung**

Nhập trước dữ liệu cho người dùng của bạn để họ không cần phải làm điều này! - Là người quản trị, bạn có thể đặt thuộc tính điện thoại và email cho người dùng của mình trước khi triển khai đặt lại mật khẩu cho tổ chức của mình. Bạn có thể thực hiện điều này bằng cách sử dụng API, PowerShell hoặc Azure AD Kết nối. Thông tin thêm tại đây:
- [Triển khai đặt lại mật khẩu mà không yêu cầu người dùng đăng ký](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Dữ liệu nào được dùng bằng cách đặt lại mật khẩu](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nút đặt lại mật khẩu bị xám**

Bạn không được phép đặt lại mật khẩu của người dùng này. Chỉ người quản trị toàn cục, mật khẩu và người dùng mới có thể đặt lại mật khẩu người dùng. Người quản trị toàn cầu cũng có thể đặt lại mật khẩu của người quản trị có đặc quyền khác.

**Tôi không thấy lưỡi đặt lại mật khẩu**

Bạn không được phép đặt lại mật khẩu. Chỉ người quản trị toàn cục, mật khẩu và người dùng mới có thể đặt lại mật khẩu người dùng. Người quản trị toàn cầu cũng có thể đặt lại mật khẩu của người quản trị có đặc quyền khác.

**Tôi không thấy lưỡi tích hợp tại chỗ trong tính năng đặt lại mật khẩu**

- Lưỡi tích hợp tại chỗ chỉ xuất hiện trong môi trường kết hợp - nghĩa là bạn đang sử dụng chức năng ghi lại mật khẩu để thao tác với mật khẩu người dùng tại chỗ.
- Bạn sẽ không thấy lưỡi này nếu:
    - Bạn đang không sử dụng chức năng ghi lại mật khẩu
    - Có sự cố với việc cài đặt/kết nối ghi lại mật khẩu của bạn
    - Đã xảy ra sự cố với việc cài đặt/kết nối Azure AD Kết nối
    - Để biết thêm các bước khắc phục sự cố ghi lại mật khẩu, hãy xem mục Khắc phục sự [cố ghi lại mật khẩu](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tôi không biết cách đặt lại mật khẩu người dùng**

1. Đăng nhập vào cổng thông tin Azure với tư cách là người quản trị thích hợp.
1. Đi đến lưỡi Người dùng và nhóm, chọn Tất **cả Người dùng**.
1. Chọn một người dùng từ danh sách.
1. Đối với người dùng đã chọn, chọn **Tổng** quan , rồi trong thanh lệnh, bấm vào Đặt **lại mật khẩu.**
1. Làm theo hướng dẫn trên màn hình.
    - Chỉ các thao tác đặt lại được thực hiện thông qua cổng thông tin Azure hỗ trợ ghi lại mật khẩu.

**Tôi đặt lại mật khẩu người dùng tại cơ sở từ cổng thông tin Office 365 Admin hoặc ứng dụng Office 365 di động nhưng người dùng vẫn không thể đăng nhập**

Chức năng Ghi lại Mật khẩu không được hỗ trợ trong cổng thông tin này. Đặt lại mật khẩu người dùng trong cổng thông tin Azure - portal.azure.com

