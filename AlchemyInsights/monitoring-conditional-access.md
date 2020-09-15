---
title: Giám sát quyền truy nhập có điều kiện
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702925"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Giám sát quyền truy nhập có điều kiện cho Exchange

Người dùng được mục tiêu với quyền truy nhập có điều kiện sẽ nhận được email thông báo nếu họ không đáp ứng các yêu cầu truy nhập của tổ chức bạn. Để giải quyết, chúng tôi khuyên bạn nên một hoặc nhiều giải pháp sau đây:
  
- Nếu thiết bị được cho là đã đăng ký, hãy tư vấn cho người dùng để đi đến ứng dụng cổng thông tin công ty và xác minh rằng nó sẽ xuất hiện trong cổng thông tin công ty. Nếu không, người dùng sẽ đăng ký thiết bị.
    
- Trong cổng thông tin Azure, đi đến ** \> tuân thủ thiết bị InTune**. Bên dưới **giám sát** bấm **tuân thủ thiết bị**. Xem báo cáo tuân thủ thiết bị của bạn để xác minh rằng thiết bị của người dùng được đánh dấu là phù hợp. 
    
- Trong cổng thông tin Azure, đi đến ** \> tuân thủ thiết bị InTune**. Bên dưới **quản lý**, bấm vào **chính sách**. Trong danh sách các chính sách tuân thủ, hãy xác nhận hồ sơ được gán cho thiết bị của người dùng. Nếu không có hồ sơ nào được phân công, thì InTune sẽ không thể xác nhận trạng thái tuân thủ của thiết bị. 
    
- Chỉnh sửa nhiệm vụ truy nhập có điều kiện của người dùng.
    
1. Trong cổng thông tin Azure, đi tới ** \> \> chính sách truy nhập InTune** có điều kiện
    
2. Chọn một chính sách từ danh sách
    
3. Bấm vào **người dùng và nhóm**
    
4. Để nhắm đến một chính sách nhất định tại một ai đó, hãy thêm họ vào danh sách **bao gồm** . Để đảm bảo rằng một người được bỏ qua khỏi chính sách, hãy thêm họ vào danh sách **loại trừ** . 
    
Đọc thêm: [cách theo dõi các thiết bị truy nhập](https://docs.microsoft.com/intune/conditional-access-exchange-monitor) có điều kiện
  

