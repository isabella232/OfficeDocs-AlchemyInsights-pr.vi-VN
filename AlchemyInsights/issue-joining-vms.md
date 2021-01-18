---
title: Sự cố khi gia nhập VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885782"
---
# <a name="issue-joining-vms"></a>Sự cố khi gia nhập VMs

Để giải quyết các sự cố xảy ra trong khi tìm cách gia nhập VMs, hãy thực hiện các bước sau đây:

1. Tìm cách đăng nhập bằng định dạng **UPN** (ví dụ: ' joeuser@contoso.com ') thay vì định dạng **SAMAccountName** (' CONTOSO\joeuser ').
2. Đảm bảo rằng bạn đã bật tính năng đồng bộ hóa mật khẩu theo các bước được nêu trong hướng dẫn *bắt đầu* .
3. Đảm bảo rằng tài khoản người dùng bị ảnh hưởng không phải là tài khoản bên ngoài trong đối tượng thuê Azure AD. Người dùng bên ngoài không thể đăng nhập vào tên miền được quản lý kể từ Azure AD Domain Services không có thông tin xác thực cho các tài khoản người dùng đó.
4. Nếu tài khoản người dùng bị ảnh hưởng là một tài khoản người dùng chỉ trên đám mây, hãy đảm bảo rằng người dùng đã thay đổi mật khẩu của họ sau khi bạn bật dịch vụ tên miền Azure AD. Bước này khiến các hàm hàm băm chứng danh bắt buộc đối với dịch vụ tên miền Azure AD sẽ được tạo ra.
5. Nếu tài khoản người dùng bị ảnh hưởng được đồng bộ từ một thư mục tại chỗ, hãy xác minh rằng bản phát hành được đề xuất của Azure AD Connect đã được cấu hình để thực hiện đồng bộ hóa đầy đủ.
6. Nếu sự cố vẫn tiếp diễn sau khi xác nhận bước 4, thực hiện các lệnh sau đây từ máy tính đồng bộ của bạn:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.