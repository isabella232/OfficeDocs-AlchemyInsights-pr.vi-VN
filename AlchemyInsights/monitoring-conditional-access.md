---
title: Giám sát điều kiện truy cập
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713740"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Giám sát điều kiện truy cập cho Exchange

Người dùng nhắm mục tiêu với truy cập có điều kiện sẽ nhận được một email thông báo nếu họ không đáp ứng yêu cầu truy cập của tổ chức bạn. Để giải quyết, chúng tôi khuyên bạn nên một hoặc nhiều giải pháp sau:
  
- Nếu thiết bị được coi là được ghi danh, hãy tư vấn cho người dùng để truy cập ứng dụng cổng thông tin công ty và xác minh rằng nó xuất hiện trong cổng thông tin công ty. Nếu không, người dùng nên đăng ký thiết bị.
    
- Trong cổng Azure đi để **InTune \> thiết bị tuân thủ**. Trong **màn hình** bấm vào **thiết bị tuân thủ**. Xem báo cáo tuân thủ thiết bị của bạn để xác minh rằng thiết bị của người dùng được đánh dấu là tuân thủ. 
    
- Trong cổng Azure đi để **InTune \> thiết bị tuân thủ**. Trong **quản lý**, bấm vào **chính sách**. Trong danh sách các chính sách tuân thủ, hãy xác minh rằng hồ sơ được gán cho thiết bị của người dùng của bạn. Nếu không có hồ sơ nào được chỉ định, thì InTune sẽ không thể xác nhận trạng thái tuân thủ của thiết bị. 
    
- Chỉnh sửa gán quyền truy cập có điều kiện của người dùng.
    
1. Trong cổng Azure đi để **InTune \> điều kiện truy \> cập chính sách**
    
2. Chọn một chính sách từ danh sách
    
3. Nhấp vào **người dùng và nhóm**
    
4. Để nhắm mục tiêu một chính sách nhất định tại một người nào đó, hãy thêm chúng vào danh sách **bao gồm** . Để đảm bảo rằng một người bị bỏ qua khỏi chính sách, hãy thêm họ vào danh sách **loại trừ** . 
    
Đọc thêm: [cách giám sát các thiết bị truy cập có điều kiện](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

