---
title: Chỉ đọc cho các thông báo bảo trì khi cố gắng sử dụng SharePoint hoặc OneDrive
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620745"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Chỉ đọc cho các thông báo bảo trì khi cố gắng sử dụng SharePoint hoặc OneDrive

Người dùng có thể nhận được một tin nhắn **Chỉ đọc bảo trì** khi cố gắng sử dụng SharePoint hoặc OneDrive cho một trong các trường hợp sau. 

-   Một kế hoạch hoặc hoạt động duy trì hoạt động.  Kiểm tra cho họ bằng cách điều hướng đến [Trung tâm tin nhắn](https://portal.office.com/adminportal/home#/messagecenter).
-   Một ưu tiên cao, hoạt động sự cố có thể xảy ra. Kiểm tra bất kỳ tư vấn/sự cố bằng cách điều hướng đến [Dịch vụ sức khỏe](https://portal.office.com/adminportal/home#/servicehealth).
-   Một tiểu tự chữa bệnh phục hồi tình huống có thể xảy ra do sự kiện bất ngờ nào trên các máy chủ đó có thể cuối cùng trong chưa đầy 30 phút hoặc lâu hơn. 
    
    Không có không có trung tâm tin nhắn hoặc dịch vụ sức khỏe bài viết cho những phục hồi nhỏ, nhưng bạn nên trở lại bình thường rất sớm.

Trong những dịp rất ít chúng tôi quan sát thấy rằng một trong ba trường hợp nêu trên có là nguyên nhân, và dịch vụ đã được khôi phục, nhưng bộ nhớ cache trình duyệt của người dùng đã bị xoá sổ.

Hãy cố gắng để xóa bộ nhớ cache của trình duyệt trước khi điều hướng đến trang web.

1. Trong trình duyệt Microsoft Edge, chọn **Settings**và sau đó chọn **quyền riêng tư và bảo mật**.
2. **Rõ ràng đang duyệt**, chọn **lựa chọn những gì để xóa**.
3. Chọn **cookie và dữ liệu trang web đã lưu**, và chọn **xóa**.

>[!Note] 
> Các bước này có thể khác biệt khi sử dụng các trình duyệt khác như Mozilla Firefox hoặc Google Chrome.

>[!Note] 
> Một tùy chọn khác sẽ là mở OneDrive hoặc SharePoint trang web của bạn trong một cửa sổ InPrivate mới.