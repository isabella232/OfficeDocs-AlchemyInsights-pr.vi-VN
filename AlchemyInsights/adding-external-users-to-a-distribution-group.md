---
title: Thêm người dùng bên ngoài vào một nhóm phân phối
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737931"
---
# <a name="add-external-users-to-a-distribution-group"></a>Thêm người dùng bên ngoài vào nhóm phân phối

Thêm một liên hệ bên ngoài vào một nhóm phân phối (DG) là một quá trình hai bước:
  
1. Tạo một liên hệ thư cho người dùng bên ngoài:
    
    1. Trong Trung tâm quản trị, hãy truy cập trang[danh bạ](https://admin.microsoft.com/adminportal/home#/Contact) **người dùng** > . 
    
    2. Chọn **Thêm một liên lạc**.
    
    3. Nhập thông tin cho liên hệ của bạn và chọn **Thêm**.
    
2. Thêm liên hệ thư vào DG của bạn:
    
    1. Trong Trung tâm quản trị, hãy chuyển **** > [đến trang nhóm](https://admin.microsoft.com/adminportal/home#/groups) nhóm. 
    
    2. Tìm DG bạn muốn thêm người dùng bên ngoài vào, và chọn nó để mở hộp thoại chỉnh sửa.
    
    3. Trên tab **thành viên** , chọn **xem tất cả và quản lý thành viên**. 
    
    4. Chọn **thêm thành viên**.
    
    5. Chọn liên hệ thư bạn đã tạo ở bước trước, sau đó chọn **lưu**.
    
Nếu sau khi làm theo các bước này người dùng bên ngoài không thể gửi email đến DG hoặc không nhận được email từ nó, có thể là DG được đánh dấu để chỉ cho phép email từ người dùng nội bộ. Bạn có thể kiểm tra cấu hình này và sửa chữa nó theo các hướng dẫn [ở đây](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Lưu ý:** Các hướng dẫn này không áp dụng nếu loại nhóm của bạn là "Office 365 nhóm" thay vì "nhóm phân phối". Nếu đó là trường hợp, bạn có thể thêm người dùng bên ngoài trực tiếp vào nhóm từ Outlook. Thông tin chi tiết về văn phòng 365 nhóm khách cũng như hướng dẫn Thêm khách bên ngoài có thể được tìm thấy trong [bài viết này](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  