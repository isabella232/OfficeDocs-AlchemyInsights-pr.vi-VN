---
title: Hành vi Cyguid/Sourceneo nhất quán
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817014"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Hành vi Cyguid/Sourceneo nhất quán

Azure AD Connect (Phiên bản 1.1.524.0 và sau) bây giờ tạo điều kiện sử dụng các Cyguid gắn kết với tên thuộc tính sourceAnchor. Khi sử dụng tính năng này, Azure AD kết nối sẽ tự động cấu hình các quy tắc đồng bộ hóa để:
  
- Sử dụng msDS-chỗ phân vị là thuộc tính sourceAnchor cho đối tượng người dùng. ObjectGUID được dùng cho các kiểu đối tượng khác.
    
- Đối với bất kỳ đối tượng người dùng quảng cáo tại cơ sở nào có thuộc tính Cyds-mâu thuẫn không có hàm, Azure AD kết nối sẽ viết giá trị objectGUID của nó trở về thuộc tính Cyguid nhất quán trong Active Directory tại chỗ. Sau đó thuộc tính Cyds-mâu thuẫn, hãy kết nối Azure AD sau đó xuất ra đối tượng Azure AD.
    
 **Lưu ý:** Sau khi đối tượng quảng cáo tại cơ sở được nhập vào Azure AD Connect (tức là, được nhập vào không gian kết nối quảng cáo và dự kiến vào metaverse), bạn không thể thay đổi giá trị Sourceneo của nó nữa. Để xác định giá trị sourceAnchor cho đối tượng quảng cáo tại cơ sở đã cho, hãy đặt cấu hình thuộc tính người dùng đồng bộ của msDS trước khi nó được nhập vào Azure AD Connect. 
  
Để biết thêm thông tin về phần giới thiệu về SourceAnchor và mâu thuẫn, hãy tham khảo các thao tác sau: [AZURE AD Connect: khái niệm thiết kế](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

