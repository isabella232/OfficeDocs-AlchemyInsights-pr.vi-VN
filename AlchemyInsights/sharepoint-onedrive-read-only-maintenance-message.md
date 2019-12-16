---
title: Chỉ đọc cho thông báo bảo trì khi cố gắng sử dụng SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051303"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Chỉ đọc cho thông báo bảo trì khi cố gắng sử dụng SharePoint hoặc OneDrive

Người dùng có thể nhận được thông báo **bảo trì chỉ đọc** khi cố gắng sử dụng SharePoint hoặc OneDrive cho một trong các trường hợp sau. 

-   Một hoạt động bảo trì kế hoạch hoặc hoạt động.  Kiểm tra chúng bằng điều hướng đến [Trung tâm thông báo](https://portal.office.com/adminportal/home#/messagecenter).
-   Một sự cố dịch vụ ưu tiên cao, hoạt động có thể xảy ra. Kiểm tra bất kỳ lời khuyên/sự cố nào bằng việc điều hướng đến [dịch vụ y tế](https://portal.office.com/adminportal/home#/servicehealth).
-   Một tình huống khôi phục tự động chữa bệnh nhỏ có thể xảy ra do bất kỳ sự kiện bất ngờ trên các máy chủ có thể kéo ít hơn 30 phút hoặc lâu hơn. 
    
    Không có trung tâm thông báo hoặc dịch vụ y tế bài viết cho các phục hồi nhỏ nhưng bạn nên trở lại bình thường rất sớm.

Trong những dịp rất ít chúng tôi quan sát thấy rằng một trong ba kịch bản được liệt kê ở trên đã được nguyên nhân, và dịch vụ đã được khôi phục, nhưng bộ nhớ cache của trình duyệt người dùng đã không được xóa.

Hãy cố gắng xóa bộ nhớ cache của trình duyệt trước khi điều hướng đến trang web.

1. Trong trình duyệt Microsoft Edge, chọn **cài đặt**, sau đó chọn **quyền riêng tư và bảo mật**.
2. Trong **xóa duyệt**, chọn **chọn nội dung cần xóa**.
3. Chọn **cookie và dữ liệu trang web đã lưu**và chọn **xóa**.

>[!Note] 
> Các bước này có thể khác nhau khi sử dụng các trình duyệt khác như Mozilla Firefox hoặc Google Chrome.

>[!Note] 
> Một tùy chọn khác sẽ là mở trang web SharePoint của bạn hoặc OneDrive trong một cửa sổ InPrivate mới.