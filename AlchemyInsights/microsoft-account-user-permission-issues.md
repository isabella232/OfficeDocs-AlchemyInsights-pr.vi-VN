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
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717368"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Gỡ rối các vấn đề - không tìm thấy người dùng trong thư mục

<p>Nếu người dùng nhận được thông báo lỗi <strong> &ldquo; &hellip;người sử dụng có thể&rsquo;t được tìm thấy trong thư mục. Xin vui lòng thử lại&hellip; </strong> nơi mà các loại vấn đề là <strong> &ldquo;người dùng không có trong thư mục.&rdquo;</strong>, theo các bước sau có thể được hoàn thành để khắc phục vấn đề.</p> <ol> <li>Đảm bảo tài khoản có chấp nhận lời mời email cùng một tài khoản đang được sử dụng để đăng nhập sau. Đảm bảo rằng người dùng đang sử dụng cùng một tài khoản để chấp nhận lời mời và đăng nhập vào trang web. <br /><br />Để biết thêm chi tiết, hãy xem <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">làm thế nào để quản lý các bí danh cho tài khoản Microsoft của bạn</a> để quản lý các đăng nhập Office 365. <br /><br /></li> <li>Trình duyệt cho mỗi trang web mà người dùng nhận được các lỗi. <br /><br />một. Thêm <strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid=0&rdquo; </strong> (trong các kép, dấu ngoặc kép) vào cuối URL của trang web. <br /><br />Ví dụ: https://&lt;contoso&gt;.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 <br /><br />b. Chọn người dùng từ danh sách. <br /><br />c. Nhấp vào <strong>xoá người sử dụng quyền hạn từ Ribbon</strong>. <br /><br />d. Thêm về người dùng và gửi lại mời cho người dùng.</li> </ol>

