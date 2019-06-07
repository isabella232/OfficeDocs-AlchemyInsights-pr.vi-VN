---
title: Tạo và sử dụng hộp thư dùng chung
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81bf8082198de1c44037291f23c434d06a77f02a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762422"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Gỡ rối các vấn đề - không tìm thấy người dùng trong thư mục

Nếu người dùng nhận được lỗi thông báo "không thể được tìm thấy người dùng" trong thư mục. Hãy thử một lần nữa nơi loại vấn đề là người dùng không phải trong thư mục.

Các bước sau đây có thể được hoàn thành để khắc phục vấn đề.

- Đảm bảo tài khoản có chấp nhận lời mời email cùng một tài khoản đang được sử dụng để đăng nhập sau. Đảm bảo rằng người dùng đang sử dụng cùng một tài khoản để chấp nhận lời mời và đăng nhập vào trang web. 

Để biết thêm thông tin, hãy xem [làm thế nào để quản lý các bí danh cho tài khoản Microsoft của bạn</a> để quản lý các đăng nhập Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Trình duyệt cho mỗi trang web mà người dùng nhận được các lỗi. 

Thêm "/ _layouts/15/people.aspx/membershipgroupid=0" (trong các kép, dấu ngoặc kép) vào cuối URL của trang web. 

Ví dụ: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Chọn người dùng từ danh sách.

- Nhấp vào **xoá người sử dụng quyền hạn** từ Ribbon. 
-  Thêm về người dùng và gửi lại mời cho người dùng.

