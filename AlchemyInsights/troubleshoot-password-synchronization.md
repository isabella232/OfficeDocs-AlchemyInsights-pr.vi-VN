---
title: Khắc phục sự cố đồng bộ hóa mật khẩu
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387899"
---
# <a name="troubleshoot-password-synchronization"></a>Khắc phục sự cố đồng bộ hóa mật khẩu

Để khắc phục sự cố đồng bộ hóa mật khẩu, khởi động bằng cách sử dụng công việc khắc phục sự cố AAD kết nối này để xác định lý do mật khẩu không đồng bộ hoá. Để bắt đầu, hãy đi tới [quản lý đồng bộ trực tiếp](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Mở phiên Windows PowerShell mới trên máy chủ Azure AD kết nối của bạn và chọn tuỳ chọn **chạy như quản trị viên** .

2. Chạy thiết lập ExecutionPolicy RemoteSigned hoặc Set-ExecutionPolicy không hạn chế.

3. Khởi động thuật sĩ Azure AD kết nối.

4. Truy cập trang tác vụ bổ sung > **khắc phục sự cố**  >  **tiếp theo**.

5. Chọn **khởi chạy** để mở menu khắc phục sự cố PowerShell.

6. Chọn **khắc phục sự cố đồng bộ hóa mật khẩu**.

    Vấn đề thường là mật khẩu không đồng bộ hoá tài khoản người dùng cụ thể.

    **Ghi chú** Đồng bộ hóa mật khẩu không thành công nếu đồng bộ hoá mật khẩu thành công cuối cùng là một số thời gian trước đây.

Để được trợ giúp thêm khắc phục sự cố đồng bộ hóa mật khẩu, xem [khắc phục sự cố đồng bộ hóa mật khẩu băm AZURE AD kết nối đồng bộ](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).