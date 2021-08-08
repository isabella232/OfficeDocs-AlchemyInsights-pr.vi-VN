---
title: Thêm người dùng bên ngoài vào một Nhóm Phân phối
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934855"
---
# <a name="add-external-users-to-a-distribution-group"></a>Thêm người dùng bên ngoài vào một Nhóm Phân phối

Thêm một liên hệ bên ngoài vào một Nhóm Phân phối (DG) là một quy trình gồm hai bước:
  
1. Tạo Liên hệ Thư cho người dùng bên ngoài:
    
    1. Trong trung tâm quản trị, đi đến trang **Liên**  >  [hệ Người](https://admin.microsoft.com/adminportal/home#/Contact) dùng. 
    
    2. Chọn **Thêm liên hệ**.
    
    3. Nhập thông tin cho liên hệ của bạn và chọn **Thêm**.
    
2. Thêm Liên hệ Thư vào DG của bạn:
    
    1. Trong trung tâm quản trị, đi đến **trang**  >  [Nhóm.](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Tìm kiếm DG bạn muốn thêm người dùng bên ngoài, rồi chọn DG đó để mở hộp thoại chỉnh sửa.
    
    3. Trên tab Thành **viên,** chọn Xem **tất cả và quản lý thành viên.** 
    
    4. Chọn **Thêm thành viên**.
    
    5. Chọn Liên hệ Thư bạn đã tạo ở bước trước đó, rồi chọn **Lưu**.
    
Nếu sau khi làm theo các bước này, người dùng bên ngoài của bạn không thể gửi email tới DG hoặc không nhận được email từ đó, có thể DG đã được đánh dấu để chỉ cho phép email từ người dùng nội bộ. Bạn có thể kiểm tra cấu hình này và khắc phục theo hướng dẫn [tại đây.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)
  
 **Lưu ý:** Không áp dụng các hướng dẫn này nếu loại nhóm của bạn là "nhóm Microsoft 365" thay vì "Nhóm phân phối". Nếu vậy, bạn có thể thêm người dùng bên ngoài trực tiếp vào nhóm từ Outlook. Bạn có thể tìm thấy thông tin chi Microsoft 365 về khách nhóm Microsoft 365 cũng như hướng dẫn để thêm khách bên ngoài trong [bài viết này.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  