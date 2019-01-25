---
title: ConsistencyGuid / sourceAnchor hành vi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 80516ed9e15040475a8b65a1af98a1b561704d49
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29498540"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor hành vi

Azure quảng cáo kết nối (Phiên bản 1.1.524.0 và sau) bây giờ tạo điều kiện sử dụng msDS-ConsistencyGuid như là thuộc tính sourceAnchor. Khi sử dụng tính năng này, Azure quảng cáo kết nối tự động cấu hình các quy tắc đồng bộ hóa cho:
  
- Sử dụng msDS-ConsistencyGuid như là thuộc tính sourceAnchor cho đối tượng người dùng. ObjectGUID được sử dụng cho các loại đối tượng khác.
    
- Đối với bất kỳ cung cấp tại chỗ quảng cáo dùng đối tượng có thuộc tính msDS-ConsistencyGuid không phải là dân cư, Azure quảng cáo kết nối viết các giá trị objectGUID lại cho thuộc tính msDS ConsistencyGuid trong Active Directory tại chỗ. Sau khi các thuộc tính msDS-ConsistencyGuid dân cư đông đúc, Azure quảng cáo kết nối sau đó xuất khẩu các đối tượng để quảng cáo Azure.
    
 **Lưu ý:** Một khi một chỗ đối tượng quảng cáo nhập khẩu vào Azure quảng cáo kết nối (có nghĩa là, được nhập vào không gian kết nối AD và dự kiến vào Metaverse), bạn không thể thay đổi giá trị sourceAnchor của nó nữa. Để xác định giá trị sourceAnchor cho một cho tại chỗ quảng cáo đối tượng, cấu hình thuộc tính msDS-ConsistencyGuid của nó trước khi nó được nhập vào Azure quảng cáo kết nối. 
  
Để biết thêm chi tiết về SourceAnchor và ConsistencyGuid, tham khảo như sau: [Azure quảng cáo kết nối: thiết kế khái niệm](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

