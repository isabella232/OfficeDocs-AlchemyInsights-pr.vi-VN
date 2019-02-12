---
title: Giám sát truy cập có điều kiện
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29902391"
---
# <a name="monitoring-conditional-access"></a>Giám sát truy cập có điều kiện

Nhắm mục tiêu với điều kiện truy cập người dùng sẽ nhận được một email thông báo nếu họ không đáp ứng yêu cầu truy cập tổ chức của bạn. Để giải quyết, chúng tôi khuyên bạn nên một hoặc nhiều các giải pháp sau:
  
- Nếu thiết bị là presumed để được đăng ký, tư vấn cho người sử dụng để đi đến các ứng dụng cổng thông tin công ty và xác minh rằng nó xuất hiện trong cổng công ty. Nếu không, người dùng nên đăng ký các thiết bị.
    
- Trong các cổng Azure vào **dành \> thiết bị tuân thủ**. Trong **màn hình** nhấp vào **thiết bị tuân thủ**. Xem báo cáo của bạn tuân thủ thiết bị để kiểm chứng rằng thiết bị của người dùng được đánh dấu như tuân thủ. 
    
- Trong các cổng Azure vào **dành \> thiết bị tuân thủ**. Trong **quản lý**, bấm vào **chính sách**. Trong danh sách các chính sách phù hợp, xác minh hồ sơ được gán cho thiết bị của người dùng. Nếu hồ sơ không được phân công, sau đó dành sẽ không thể để xác nhận tình trạng tuân thủ của thiết bị. 
    
- Chỉnh sửa của người dùng truy cập có điều kiện chuyển nhượng.
    
1. Trong các cổng Azure vào **dành \> có điều kiện truy cập \> chính sách**
    
2. Chọn một chính sách từ danh sách
    
3. Nhấp vào **người dùng và nhóm**
    
4. Để nhắm mục tiêu một chính sách nhất định vào một ai đó, thêm chúng vào danh sách **bao gồm** . Để đảm bảo rằng một người bỏ qua từ chính sách, thêm chúng vào danh sách **loại trừ** . 
    
Đọc thêm: [làm thế nào để giám sát truy cập có điều kiện thiết bị](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

