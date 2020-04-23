---
title: Khắc phục sự cố đồng bộ hóa mật khẩu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732532"
---
# <a name="troubleshoot-password-synchronization"></a>Khắc phục sự cố đồng bộ hóa mật khẩu

Để khắc phục sự cố mà không có mật khẩu được đồng bộ hoá với Azure AD kết nối phiên bản 1.1.614.0 hoặc mới hơn:
  
1. Mở phiên Windows PowerShell mới trên máy chủ Azure AD kết nối với tùy chọn **chạy như quản trị viên** .

2. Chạy **thiết lập ExecutionPolicy RemoteSigned** hoặc **thiết lập ExecutionPolicy không hạn**chế.

3. Khởi động thuật sĩ Azure AD kết nối.

4. Điều hướng đến trang **tác vụ bổ sung** , chọn **khắc phục sự cố**và nhấp vào **tiếp theo**.

5. Trang khắc phục sự cố, bấm **khởi động để khởi động trình đơn khắc phục sự cố** trong PowerShell.

6. Trong menu chính, chọn **khắc phục sự cố đồng bộ hóa mật khẩu**.

7. Trong menu phụ, chọn **đồng bộ hóa mật khẩu không hoạt động ở tất cả**.

**Hiểu kết quả của tác vụ khắc phục sự cố**
  
Việc khắc phục sự cố thực hiện kiểm tra sau:
  
- Xác thực rằng tính năng đồng bộ hóa mật khẩu được kích hoạt cho thuê Azure AD.

- Xác nhận rằng Azure AD kết nối máy chủ không ở chế độ dàn.

- Đối với mỗi kết nối Active Directory tại chỗ hiện tại (tương ứng với một nhóm Active Directory hiện có):

- 
  - Xác nhận rằng tính năng đồng bộ hóa mật khẩu được kích hoạt.

  - Tìm kiếm đồng bộ hóa mật khẩu Heartbeat sự kiện trong Nhật ký sự kiện ứng dụng Windows.

  - Đối với mỗi miền Active Directory trong kết nối Active Directory tại chỗ:

  - Xác nhận tên miền có thể truy cập từ máy chủ Azure AD kết nối.

  - Xác thực rằng tài khoản Dịch vụ miền Active Directory (AD DS) sử dụng kết nối Active Directory tại chỗ có đúng tên người dùng, mật khẩu và quyền cần thiết để đồng bộ hóa mật khẩu.

Để được trợ giúp thêm khắc phục sự cố đồng bộ hóa mật khẩu, xem [khắc phục sự cố đồng bộ hóa mật khẩu với AZURE AD kết nối đồng](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)
  