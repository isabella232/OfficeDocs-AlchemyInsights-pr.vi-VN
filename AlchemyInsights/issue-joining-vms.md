---
title: Sự cố khi gia nhập máy ảo
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
ms.openlocfilehash: d89fb92ce1775e5a77808a1893a315419b4d54706dc737327c51f7c4c4e488e2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088094"
---
# <a name="issue-joining-vms"></a>Sự cố khi gia nhập máy ảo

Để giải quyết các vấn đề xảy ra trong khi tìm cách gia nhập máy ảo, hãy thực hiện các bước sau đây:

1. Cố gắng đăng nhập bằng cách dùng định dạng **UPN** (ví dụ, 'joeuser@contoso.com') thay vì định dạng **SAMAccountName** ('CONTOSO\joeuser').
2. Đảm bảo rằng bạn đã bật đồng bộ hóa mật khẩu theo các bước được nêu trong hướng *dẫn Bắt* đầu.
3. Đảm bảo rằng tài khoản người dùng bị ảnh hưởng không phải là tài khoản bên ngoài trong đối tượng thuê Azure AD. Người dùng bên ngoài không thể đăng nhập vào miền được quản lý vì Azure AD Domain Services không có thông tin xác thực cho tài khoản người dùng này.
4. Nếu tài khoản người dùng bị ảnh hưởng là tài khoản người dùng chỉ trên đám mây, hãy đảm bảo rằng người dùng đã thay đổi mật khẩu sau khi bạn bật Azure AD Domain Services. Bước này sẽ yêu cầu tạo các hàm hashes thông tin xác thực cho Azure AD Domain Services.
5. Nếu tài khoản người dùng bị ảnh hưởng được đồng bộ hóa từ thư mục tại chỗ, hãy xác minh rằng bản phát hành đề xuất của Azure AD Kết nối đã được đặt cấu hình để thực hiện đồng bộ hóa đầy đủ.
6. Nếu sự cố vẫn tiếp diễn sau khi xác nhận Bước 4, hãy thực hiện các lệnh sau từ máy đồng bộ của bạn:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.