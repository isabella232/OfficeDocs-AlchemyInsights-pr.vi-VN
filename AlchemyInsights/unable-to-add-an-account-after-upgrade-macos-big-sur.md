---
title: Không thể thêm tài khoản sau khi nâng cấp lên macOS 11.6 Big Sur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506762"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Không thể thêm tài khoản sau khi nâng cấp lên macOS 11.6 Big Sur

Sau khi nâng cấp lên macOS 11.6, OneDrive cho tài khoản cơ quan hoặc trường học hoặc tài khoản OneDrive cá nhân của bạn có thể không xuất hiện trong danh sách tài khoản của bạn và bạn có thể không đăng nhập vào tài khoản thứ hai từ ứng dụng.

Bản sửa lỗi đã được phát triển cho sự cố này. Trước tiên, hãy xác định xem liệu bạn đang chạy phiên bản độc lập hay App Store của OneDrive:

- Chọn đám OneDrive trên thanh menu để xem > **Trợ giúp & Cài đặt** Tùy chọn  >  **Giới**  >  **thiệu.** Nếu số phiên bản không bao gồm **(Độc lập),** thì bạn đã có phiên bản App Store của sản phẩm.

Nếu bạn đang sử dụng phiên bản độc lập của OneDrive, hãy khởi động lại máy tính của bạn và cập nhật tự động OneDrive lên bản dựng mà tại đó sự cố này được giải quyết. Nếu bạn muốn cài đặt bản dựng theo cách thủ công, hãy tải xuống tệp [.zip](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)này , giải nén tệp và sao chép ứng dụng OneDrive vào thư mục Ứng dụng (bằng cách thay thế ứng dụng OneDrive hiện có).

Nếu bạn đang sử dụng phiên bản App Store, hãy cân nhắc cài đặt phiên bản độc lập của ứng dụng OneDrive. Phiên bản này hoạt động giống như phiên bản App Store nhưng cho phép Microsoft cung cấp các bản cập nhật nhanh hơn cho người dùng và kết nối họ với phiên bản có bản sửa lỗi cho sự cố này.

1. Tải xuống phiên bản độc lập của OneDrive [bản sửa lỗi .](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)
2. Giải nén tệp, rồi sao chép ứng dụng OneDrive vào thư mục Ứng dụng (bằng cách thay thế tệp hiện OneDrive dụng).

Nếu bạn cần sử dụng phiên bản App Store, hãy chờ App Store phát hành phiên bản ứng dụng có bao gồm bản sửa lỗi. Rất tiếc, Microsoft không thể thông báo ngày ước tính cho một phiên bản cố định được phát hành từ App Store.


