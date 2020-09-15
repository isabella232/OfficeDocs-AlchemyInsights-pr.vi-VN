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
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664948"
---
# <a name="troubleshoot-password-synchronization"></a>Khắc phục sự cố đồng bộ hóa mật khẩu

Để khắc phục sự cố về đồng bộ hóa mật khẩu, hãy bắt đầu bằng cách sử dụng tác vụ khắc phục sự cố kết nối này để xác định tại sao mật khẩu không đồng bộ. Để bắt đầu, hãy đi đến [quản lý đồng bộ trực tiếp](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Mở phiên Windows PowerShell mới trên máy chủ Azure AD Connect của bạn, rồi chọn tùy chọn **chạy với tư cách người quản trị** .

2. Chạy Set-ExecutionPolicy RemoteSigned hoặc Set-ExecutionPolicy không hạn chế.

3. Khởi động trình hướng dẫn Azure AD Connect.

4. Đi đến trang nhiệm vụ bổ sung > **khắc phục sự cố**  >  **tiếp theo**.

5. Chọn **khởi động** để mở menu khắc phục sự cố PowerShell.

6. Chọn **khắc phục sự cố đồng bộ hóa mật khẩu**.

    Vấn đề thường là một mật khẩu không được đồng bộ cho một tài khoản người dùng cụ thể.

    **Ghi chú** Đồng bộ hóa mật khẩu không thể nếu đồng bộ mật khẩu đã thành công cuối cùng đã được một thời gian trước đây.

Để biết thêm trợ giúp khắc phục sự cố đồng bộ hóa mật khẩu, hãy xem [khắc phục sự cố đồng bộ hóa băm mật khẩu với AZURE AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).