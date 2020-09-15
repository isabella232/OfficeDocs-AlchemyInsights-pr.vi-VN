---
title: Thêm người dùng bên ngoài vào một nhóm phân phối
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663535"
---
# <a name="add-external-users-to-a-distribution-group"></a>Thêm người dùng bên ngoài vào một nhóm phân phối

Thêm một liên hệ bên ngoài vào một nhóm phân phối (DG) là quy trình hai bước:
  
1. Tạo liên hệ thư cho người dùng bên ngoài:
    
    1. Trong Trung tâm quản trị, đi tới **Users**  >  trang[liên hệ](https://admin.microsoft.com/adminportal/home#/Contact) của người dùng. 
    
    2. Chọn **Thêm liên hệ**.
    
    3. Nhập thông tin cho liên hệ của bạn, rồi chọn **Thêm**.
    
2. Thêm liên hệ thư vào DG của bạn:
    
    1. Trong Trung tâm quản trị, đi tới **Groups**  >  trang[nhóm](https://admin.microsoft.com/adminportal/home#/groups) nhóm. 
    
    2. Tìm DG bạn muốn thêm người dùng bên ngoài, rồi chọn nó để mở hộp thoại chỉnh sửa.
    
    3. Trên tab **thành viên** , hãy chọn **xem tất cả và quản lý thành viên**. 
    
    4. Chọn **thêm thành viên**.
    
    5. Chọn liên hệ thư bạn đã tạo ở bước trước, rồi chọn **lưu**.
    
Nếu sau khi làm theo các bước này, người dùng bên ngoài của bạn không thể gửi email đến DG hoặc không nhận được email từ nó, thì có thể là DG được đánh dấu là chỉ cho phép các email từ người dùng nội bộ. Bạn có thể kiểm tra cấu hình này và sửa nó theo các hướng dẫn [ở đây](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Lưu ý:** Những hướng dẫn này không áp dụng nếu loại nhóm của bạn là "nhóm Microsoft 365" thay vì "nhóm phân phối". Nếu đó là trường hợp, bạn có thể thêm người dùng bên ngoài trực tiếp vào nhóm từ Outlook. Thông tin chi tiết về các nhóm Microsoft 365 cũng như các hướng dẫn cho việc thêm khách bên ngoài có thể tìm thấy trong [bài viết này](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  