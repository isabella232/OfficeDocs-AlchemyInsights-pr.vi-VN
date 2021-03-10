---
title: Vấn đề đặt lại mật khẩu
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
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696283"
---
# <a name="problems-resetting-password"></a>Các vấn đề về việc đặt lại mật khẩu

Sau đây là một số vấn đề mà bạn có thể gặp phải khi đặt lại mật khẩu và các giải pháp có thể xảy ra:

**Tôi đang gặp vấn đề với việc đặt lại mật khẩu không được bảo vệ trong các thể loại khác**

- Đảm bảo bạn được ủy quyền để đặt lại mật khẩu. Chỉ có người quản trị toàn cầu, mật khẩu và người dùng có thể đặt lại mật khẩu người dùng. Người quản trị toàn cầu cũng có thể đặt lại mật khẩu của người quản trị đặc quyền khác.
- Đảm bảo rằng bạn hiểu được các yêu cầu cấp phép:
    - Bạn phải có ít nhất một giấy phép được gán trong tổ chức của bạn
        - Đám mây chỉ người dùng-bất kỳ Office 365 (O365) được trả về SKU hoặc Azure AD BASIC
        - Nền tảng điện toán đám mây và/hoặc người dùng tại cơ sở-Azure AD Premium P1 hoặc P2, doanh nghiệp Mobility + Security (EMS), hoặc doanh nghiệp hiệu quả bảo mật (SPE)
        - Để đọc thêm về các yêu cầu cấp phép, hãy xem bài viết các [yêu cầu cấp phép cho AZURE AD tự đặt lại mật khẩu](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).

**Tôi đang gặp vấn đề khi kiểm tra chính sách đặt lại mật khẩu tôi đặt**

- Các chính sách được áp dụng gần đây có thể mất vài phút để sao chép trên tất cả các trung tâm dữ liệu và điểm cuối. Khoảng cách vật lý từ Trung tâm dữ liệu cũng sẽ ảnh hưởng đến cách áp dụng các thay đổi nhanh chóng.
- Kiểm tra với người dùng cuối, chứ không phải là người quản trị và thí điểm có một tập hợp người dùng nhỏ. Các chính sách được cấu hình trong cổng thông tin Azure chỉ áp dụng cho người dùng cuối, chứ không phải người quản trị. Microsoft hỗ trợ một chính sách đặt lại mật khẩu hai cổng mặc định mạnh cho bất kỳ vai trò người quản trị Azure nào (ví dụ: người quản trị toàn cầu, người quản trị, người quản trị mật khẩu, v.v.)
    - Tìm hiểu thêm về [chính sách dành cho người quản trị](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**Tôi muốn triển khai đặt lại mật khẩu nhưng không muốn người dùng của tôi đăng ký thông tin bảo mật bổ sung**

Dữ liệu trước khi cư trú cho người dùng của bạn để họ không có! -Với tư cách là người quản trị, bạn có thể đặt các thuộc tính điện thoại và email cho người dùng của bạn trước khi đặt lại mật khẩu cho tổ chức của bạn. Bạn có thể thực hiện điều này bằng cách dùng API, PowerShell hoặc Azure AD Connect. Xem thêm thông tin tại đây:
- [Triển khai việc đặt lại mật khẩu mà không yêu cầu người dùng đăng ký](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Việc đặt lại mật khẩu, dữ liệu nào được sử dụng](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nút đặt lại mật khẩu bị mờ đi**

Bạn không được phép đặt lại mật khẩu của người dùng này. Chỉ có người quản trị toàn cầu, mật khẩu và người dùng có thể đặt lại mật khẩu người dùng. Người quản trị toàn cầu cũng có thể đặt lại mật khẩu của người quản trị đặc quyền khác.

**Tôi không nhìn thấy lưỡi đặt lại mật khẩu**

Bạn không được phép đặt lại mật khẩu. Chỉ có người quản trị toàn cầu, mật khẩu và người dùng có thể đặt lại mật khẩu người dùng. Người quản trị toàn cầu cũng có thể đặt lại mật khẩu của người quản trị đặc quyền khác.

**Tôi không nhìn thấy lưỡi kiếm tích hợp tại cơ sở trong đặt lại mật khẩu**

- Lưỡi tích hợp tại cơ sở chỉ xuất hiện trong môi trường hỗn hợp-nghĩa là bạn đang sử dụng writeback để thao tác mật khẩu của người dùng tại cơ sở.
- Bạn không thấy lưỡi này nếu:
    - Bạn không sử dụng writeback mật khẩu
    - Có vấn đề với việc cài đặt/kết nối của writeback mật khẩu
    - Có vấn đề với việc cài đặt/kết nối của Azure AD Connect
    - Để biết thêm các bước khắc phục sự cố với mật khẩu trở lại, hãy xem mục [khắc phục sự cố về mật khẩu](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tôi không biết làm thế nào để đặt lại mật khẩu người dùng**

1. Đăng nhập vào cổng thông tin Azure với tư cách là người quản trị thích hợp.
1. Đi đến lưỡi người dùng và nhóm, chọn **tất cả người dùng**.
1. Chọn một người dùng từ danh sách.
1. Đối với người dùng đã chọn, hãy chọn **tổng quan**, sau đó trong thanh lệnh, hãy bấm **đặt lại mật khẩu**.
1. Làm theo hướng dẫn trên màn hình.
    - Chỉ Reset được thực hiện thông qua dịch vụ hỗ trợ Azure Portal.

**Tôi đặt lại mật khẩu người dùng tại cơ sở từ cổng thông tin quản trị Office 365 hoặc ứng dụng Office 365 dành cho thiết bị di động nhưng người dùng vẫn không thể đăng nhập**

Không hỗ trợ mật khẩu của Writeback trong cổng thông tin này. Đặt lại mật khẩu người dùng một lần nữa trong cổng thông tin Azure-portal.azure.com

