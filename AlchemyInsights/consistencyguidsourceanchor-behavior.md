---
title: Hành vi của các mâu thuẫn/sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705755"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Hành vi của các mâu thuẫn/sourceAnchor

Azure AD kết nối (Phiên bản 1.1.524.0 và sau) bây giờ tạo điều kiện cho việc sử dụng msDS, Cyguid là sourceAnchor thuộc tính. Khi sử dụng tính năng này, Azure AD kết nối tự động cấu hình các quy tắc đồng bộ hóa để:
  
- Sử dụng msDS sự nhất quán Cyguid là thuộc tính sourceAnchor đối tượng người dùng. ObjectGUID được sử dụng cho các loại đối tượng.
    
- Đối tượng cho bất kỳ chỗ AD người dùng trên cơ sở có msDS-sự nhất quán thuộc tính không được xác định, Azure AD kết nối ghi giá trị objectGUID về thuộc tính msDS-sự nhất quán trong Active Directory tại chỗ. Sau khi msDS-thuộc tính chính xác Cyguid được điền, Azure AD kết nối sau đó xuất đối tượng Azure AD.
    
 **Lưu ý:** Khi một đối tượng AD tại chỗ được nhập vào Azure AD kết nối (tức là, nhập vào không gian kết nối quảng cáo và dự kiến vào metaverse), bạn không thể thay đổi giá trị sourceAnchor nữa. Để xác định giá trị sourceAnchor cho một đối tượng quảng cáo tại chỗ, cấu hình thuộc tính msDS của các Cyguid trước khi nó được nhập vào Azure AD kết nối. 
  
Để biết thêm thông tin về SourceAnchor và sự nhất quán Cyguid, hãy tham khảo sau: [AZURE AD kết nối: thiết kế khái niệm](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

