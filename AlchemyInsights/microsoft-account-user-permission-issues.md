---
title: Khắc phục sự cố-người dùng không tìm thấy trong thư mục
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725429"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Khắc phục sự cố-người dùng không tìm thấy trong thư mục

Nếu người dùng đang nhận được thông báo lỗi "không thể tìm thấy người dùng" trong thư mục, vui lòng thử lại nơi mà kiểu vấn đề là người dùng không có trong thư mục.

Các bước sau đây có thể được hoàn tất để khắc phục sự cố này.

- Đảm bảo tài khoản chấp nhận lời mời email là cùng một tài khoản đang được sử dụng để đăng nhập sau đó. Đảm bảo rằng người dùng đang sử dụng cùng một tài khoản để chấp nhận lời mời và đăng nhập vào trang. 

Để biết thêm thông tin, hãy xem [cách quản lý biệt danh cho tài khoản Microsoft của bạn </a> để quản lý đăng nhập Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Duyệt đến từng (các) site mà người dùng đang nhận được lỗi. 

Thêm "/_layouts/15/17/người. aspx/membershipgroupid = 0" (trong dấu ngoặc kép) đến cuối URL của site. 

Ví dụ: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Chọn người dùng từ danh sách.

- Bấm **loại bỏ quyền của người dùng** khỏi dải băng. 
-  Thêm lại người dùng và gửi lại lời mời cho người dùng.

