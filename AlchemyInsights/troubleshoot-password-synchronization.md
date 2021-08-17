---
title: Khắc phục sự cố đồng bộ hóa mật khẩu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105800"
---
# <a name="troubleshoot-password-synchronization"></a>Khắc phục sự cố đồng bộ hóa mật khẩu

Để khắc phục sự cố đồng bộ hóa mật khẩu, hãy bắt đầu bằng cách sử dụng AAD này để Kết nối cố khắc phục sự cố để xác định lý do mật khẩu không đồng bộ. Để bắt đầu, hãy đi tới Quản [lý đồng bộ trực tiếp](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Mở một phiên làm Windows PowerShell trên máy chủ azure AD Kết nối của bạn, rồi chọn tùy chọn **Chạy với vai trò Người quản** trị.

2. Chạy Set-ExecutionPolicy ký từ xa hoặc Set-ExecutionPolicy Hạn chế.

3. Khởi động trình hướng dẫn Kết nối Azure AD.

4. Đi đến trang Nhiệm vụ Bổ sung để > **khắc phục sự cố tiếp**  >  **theo**.

5. Chọn **Khởi** chạy để mở menu khắc phục sự cố PowerShell.

6. Chọn **Khắc phục sự cố Đồng bộ hóa Mật khẩu**.

    Vấn đề thường là mật khẩu không được đồng bộ hóa cho một tài khoản người dùng cụ thể.

    **Ghi chú** Đồng bộ hóa mật khẩu không thành công nếu lần đồng bộ mật khẩu thành công gần đây nhất đã xảy ra cách đây một thời gian.

Để biết thêm trợ giúp khắc phục sự cố đồng bộ hóa mật khẩu, hãy xem mục Khắc phục sự cố đồng bộ hóa băm mật khẩu [với Azure AD Kết nối đồng bộ](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).