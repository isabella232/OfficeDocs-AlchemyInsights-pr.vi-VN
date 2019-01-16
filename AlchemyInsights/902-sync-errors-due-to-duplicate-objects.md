---
title: 902 (sync lỗi do các đối tượng trùng lặp)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28320983"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Lỗi đồng bộ hóa do các đối tượng trùng lặp

Bạn có thể nhận được một trong các thông báo lỗi sau khi đồng bộ hoá thư mục kết thúc:
  
- Không thể cập nhật các đối tượng này ở Microsoft dịch vụ trực tuyến bởi vì các thuộc tính sau đây liên quan đến đối tượng này có giá trị có thể đã được liên kết với các đối tượng khác trong thư mục địa phương của bạn.
    
- Một đối tượng được đồng bộ hoá với cùng một địa chỉ proxy đã tồn tại trong thư mục Microsoft dịch vụ trực tuyến của bạn.
    
- Không thể cập nhật các đối tượng này bởi vì các thuộc tính sau đây liên quan đến đối tượng này có giá trị mà có thể đã được liên kết với các đối tượng khác trong dịch vụ thư mục địa phương của bạn: UserPrincipalName.
    
Để xác định và khắc phục sự cố, hãy tải về và chạy [Công cụ khắc phục lỗi IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).
  
Để biết thêm thông tin, hãy xem [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
  
