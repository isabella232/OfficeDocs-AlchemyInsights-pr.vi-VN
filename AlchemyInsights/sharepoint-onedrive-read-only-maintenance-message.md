---
title: Read-Only cho thông báo Bảo trì khi tìm cách sử dụng SharePoint thiết bị OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: edcdea2f5c0647b92c230dd1d86549173e72997fc885195cde688b3b17710a2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910568"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only cho thông báo Bảo trì khi tìm cách sử dụng SharePoint thiết bị OneDrive

Người dùng có thể nhận **được** thông báo Chỉ Đọc cho Bảo trì khi tìm cách sử dụng SharePoint hoặc OneDrive cho một trong các kịch bản sau đây. 

-   Một hoạt động bảo trì theo kế hoạch hoặc hiện hoạt.  Kiểm tra thiết bị bằng cách dẫn hướng đến Trung [tâm Thông báo](https://portal.office.com/adminportal/home#/messagecenter).
-   Một sự cố dịch vụ hiện hoạt được ưu tiên cao có thể xảy ra. Kiểm tra bất kỳ tư vấn/sự cố nào bằng cách dẫn hướng tới [Tình trạng Dịch vụ](https://portal.office.com/adminportal/home#/servicehealth).
-   Kịch bản khôi phục sức khỏe tự động phục hồi nhỏ có thể xảy ra do bất kỳ sự kiện không mong muốn nào trên các máy chủ có thể kéo dài trong ít hơn 30 phút trở lên. 
    
    Không có bài đăng Trung tâm Thông báo hoặc Trạng thái Dịch vụ cho những khôi phục nhỏ này nhưng bạn sẽ sớm trở lại bình thường.

Trong rất ít trường hợp chúng tôi quan sát được rằng một trong ba kịch bản được liệt kê ở trên là nguyên nhân và dịch vụ đã được khôi phục, nhưng bộ đệm ẩn trình duyệt người dùng chưa bị xóa.

Vui lòng cố xóa bộ đệm ẩn của trình duyệt trước khi dẫn hướng tới site đó.

1. Trong trình duyệt Microsoft Edge quan của bạn, **chọn Cài đặt**, sau đó chọn Quyền riêng tư và **Bảo mật**.
2. Trong **xóa duyệt**, chọn Chọn nội dụng cần **xóa**.
3. Chọn **Cookie và dữ liệu trang web đã lưu**, rồi chọn **Xóa**.

>[!Note] 
> Các bước này có thể khác khi sử dụng các trình duyệt khác như Mozilla Firefox hoặc Google Chrome.

>[!Note] 
> Một tùy chọn khác là mở trang SharePoint hoặc OneDrive của bạn trong cửa sổ InPrivate mới.