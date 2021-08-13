---
title: Xóa kênh Teams riêng tư
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
ms.openlocfilehash: 33bf8a5cdc3a8e8da78c9d02e11387a778a7acce483e4485f595d9e05b344433
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948293"
---
# <a name="delete-a-teams-private-channel"></a>Xóa kênh Teams riêng tư

Microsoft đã biết về sự cố khi xóa kênh Teams riêng tư nếu bạn đã bật Chính sách Duy SharePoint ẩn cho site SharePoint ẩn. Microsoft đang nỗ lực tạo bản sửa lỗi. Trong lúc này, bạn có thể sử dụng các giải pháp thay thế sau đây để xóa kênh riêng tư.

**Loại trừ tuyển tập Nhóm/site khỏi chính sách duy trì Sharepoint.**

1. Đi đến cổng thông Office 365 quản trị của bạn, rồi chọn **Hiển thị tất cả** trong ngăn dẫn hướng bên trái.
2. Bên dưới **Trung tâm quản trị**, đi tới mục Bảo & chính sách **ngăn** mất dữ liệu  >  **tuân**  >  **thủ**.
3. Xác định bất kỳ chính sách nào áp dụng cho các site Sharepoint và sửa đổi chính sách để site Sharepoint cho Nhóm có chứa kênh riêng tư không được bao gồm trong chính sách duy trì.
4. Lưu chính sách.
    Có thể mất tới 24 giờ để thiết đặt chính sách có hiệu lực.
    Sau khi site bị loại trừ, bạn có thể xóa kênh riêng tư đó.  
    
Bạn ***có thể*** xóa kênh riêng tư bằng cách sử dụng Microsoft Teams trên thiết bị Android của mình. 

Để biết thông SharePoint liên quan, hãy xem Không thể xóa mục [trong SharePoint Online hoặc OneDrive for Business.](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)