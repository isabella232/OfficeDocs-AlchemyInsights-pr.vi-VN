---
title: Khắc phục sự cố - Không tìm thấy người dùng trong thư mục
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098192"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Khắc phục sự cố - Không tìm thấy người dùng trong thư mục

Nếu người dùng nhận được thông báo lỗi "không thể tìm thấy người dùng" trong thư mục, vui lòng thử lại nơi Loại Sự cố là Người dùng không có trong thư mục.

Bạn có thể hoàn tất các bước sau đây để khắc phục sự cố.

- Đảm bảo tài khoản đã chấp nhận lời mời email là cùng một tài khoản đang được sử dụng để đăng nhập sau này. Hãy đảm bảo rằng người dùng đang sử dụng cùng một tài khoản để chấp nhận lời mời và đăng nhập vào site. 

Để biết thêm thông tin, [hãy xem mục Cách quản lý biệt danh cho tài khoản Microsoft của bạn để quản lý đăng </a> Microsoft 365 nhập](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Duyệt đến từng (các) site mà người dùng gặp phải lỗi trong đó. 

Thêm "/_layouts/15/people.aspx/membershipgroupid=0" (trong dấu ngoặc kép) vào cuối URL của site. 

Ví dụ: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Chọn người dùng từ danh sách.

- Bấm **Loại bỏ Quyền Người dùng** khỏi Ribbon. 
-  Thêm lại Người dùng và Gửi lại lời mời cho người dùng.

