---
title: Tạo một trang web SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1386"
- "2303"
- "5200004"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 022f572aadae3b4d9f6665f9f8be871d79b51817
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/19/2019
ms.locfileid: "35802988"
---
# <a name="create-a-sharepoint-site"></a>Tạo một trang web SharePoint

Bạn có thể thấy sau đây để biết thông tin về SharePoint trang web tạo ra:
- [Quản lý các trang web trong Trung tâm quản trị SharePoint mới](https://docs.microsoft.com/sharepoint/manage-site-creation): tìm hiểu về lựa chọn sáng tạo trang web, bao gồm làm thế nào để tạo một trang web cổ điển hoặc một trang web đội không bao gồm một nhóm Office 365.
- [Tạo một nhóm trang web trong SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): tìm hiểu làm thế nào để tạo một trang web đội ngũ.
- [Tạo một trang web thông tin liên lạc trong SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): tìm hiểu làm thế nào để tạo một trang web thông tin liên lạc.
- [Quản lý các trang web trong Trung tâm quản trị SharePoint mới](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): tìm hiểu làm thế nào để tạo một trang web cổ điển hoặc một trang web đội không bao gồm một nhóm Office 365.


  
> [! Lời khuyên]
> - Bạn không thể tạo ra một trang web với cùng một URL của một trang web hiện có. Nếu bạn xóa một trang web và có nhu cầu tái sử dụng URL, nó có thể đã bị xóa trang web vẫn còn tồn tại trong **các trang web đã bị xoá**. Để quản lý đã xoá cho xem các trang web, [xóa một trang web](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site). Để hoàn toàn loại bỏ một trang web bằng Powershell, hãy xem ví dụ lệnh ghép ngắn [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .
> - Một số người dùng không thể tạo ra một trang web. Hãy xem [quản lý tạo ra trang web trong SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).
> - Nó có thể trang web xuất hiện khó khăn lúc **tạo** dài hơn dự kiến. Nếu nhiều hơn 24 giờ đã trôi qua kể từ khi bạn lần đầu tiên thấy vấn đề này, xin vui lòng đăng nhập một vé hỗ trợ. Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp. Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn thành một giải pháp.
> - Nếu bạn cần để tạo ra một trang web mới của đội tuyển mà không bao gồm một nhóm Office 365, 


