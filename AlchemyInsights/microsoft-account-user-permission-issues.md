---
title: Khắc phục sự cố-người dùng không tìm thấy trong thư mục
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768823"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Khắc phục sự cố-người dùng không tìm thấy trong thư mục

Nếu người dùng nhận được thông báo lỗi "không thể tìm thấy người dùng" trong thư mục, vui lòng thử lại nơi loại sự cố là người dùng không có trong thư mục.

Các bước sau đây có thể được hoàn tất để khắc phục sự cố.

- Đảm bảo tài khoản chấp nhận lời mời email là cùng một tài khoản đang được sử dụng để đăng nhập sau này. Đảm bảo rằng người dùng đang sử dụng cùng một tài khoản để chấp nhận lời mời và đăng nhập vào trang web. 

Để biết thêm thông tin, hãy xem [cách quản lý bí danh</a> cho tài khoản Microsoft của bạn để quản lý văn phòng 365 đăng nhập](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Duyệt tới mỗi (các) trang web mà người dùng nhận được lỗi. 

Thêm "/_layouts/15/nhân .aspx/membershipgroupid = 0" (trong các dấu ngoặc kép) đến cuối URL trang web. 

Ví dụ: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Chọn người dùng từ danh sách.

- Bấm **loại bỏ quyền của người dùng** từ ruy băng. 
-  Thêm lùi người dùng và gửi lại lời mời cho người dùng.

