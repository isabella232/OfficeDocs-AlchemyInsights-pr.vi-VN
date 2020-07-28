---
title: Xóa kênh riêng của teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439909"
---
# <a name="delete-a-teams-private-channel"></a>Xóa kênh riêng của teams

Microsoft đã biết sự cố xoá kênh riêng teams nếu bạn có chính sách lưu giữ SharePoint cho phép các trang web SharePoint cơ bản. Microsoft đang làm việc khắc phục sự cố. Trong khi đó, bạn có thể sử dụng giải pháp sau để xoá kênh riêng.

**Loại trừ bộ sưu tập nhóm/trang web khỏi chính sách lưu giữ SharePoint.**

1. Đi tới cổng quản trị Office 365, và chọn **Hiển thị tất cả** trong ngăn điều hướng bên trái.
2. Trong **Trung tâm quản trị**, hãy truy cập chính sách ngăn ngừa mất dữ liệu **tuân thủ & bảo mật**  >  **Data Loss Prevention**  >  **Policy**.
3. Xác định bất kỳ chính sách áp dụng cho các trang web SharePoint và sửa đổi chính sách để các trang web SharePoint cho nhóm có kênh riêng không được bao gồm trong chính sách lưu giữ.
4. Lưu chính sách.
    Có thể mất đến 24 giờ để cài đặt chính sách có hiệu lực.
    Sau khi trang web đã bị loại trừ, bạn có thể xóa kênh riêng tư.  
    
Bạn ***có*** thể xóa kênh riêng bằng cách sử dụng Microsoft teams trên thiết bị Android của mình. 

Thông tin SharePoint liên quan, xem [không thể xoá các mục trong SharePoint trực tuyến hoặc OneDrive dành cho doanh nghiệp](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).