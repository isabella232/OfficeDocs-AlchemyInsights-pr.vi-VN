---
title: Xóa kênh riêng của nhóm
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730937"
---
# <a name="delete-a-teams-private-channel"></a>Xóa kênh riêng của nhóm

Microsoft đã biết về sự cố khi xóa một kênh riêng của nhóm nếu bạn đã bật các chính sách duy trì SharePoint cho site SharePoint cơ bản. Microsoft đang làm việc trên bản sửa lỗi. Trong lúc này, bạn có thể sử dụng các giải pháp thay thế sau đây để xóa kênh riêng tư.

**Loại trừ nhóm/tuyển tập trang từ chính sách duy trì SharePoint.**

1. Đi đến cổng thông tin quản trị Office 365, rồi chọn **Hiển thị tất cả** trong ngăn dẫn hướng bên trái.
2. Bên dưới **Trung tâm quản trị**, đi đến **bảo mật &**  >  chính sách**ngăn chặn dữ liệu**tuân thủ  >  **Policy**.
3. Xác định bất kỳ chính sách nào áp dụng cho các site SharePoint và sửa đổi chính sách để trang SharePoint cho nhóm có chứa kênh riêng tư không được bao gồm trong chính sách duy trì.
4. Lưu chính sách.
    Có thể mất đến 24 giờ để thiết đặt chính sách có hiệu lực.
    Sau khi site đã bị loại trừ, bạn có thể xóa kênh riêng tư.  
    
Bạn  ***có thể*** xóa kênh riêng tư bằng cách sử dụng Microsoft nhóm trên thiết bị Android của mình. 

Để biết thông tin SharePoint liên quan, hãy xem [không thể xóa các mục trong SharePoint Online hoặc OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).