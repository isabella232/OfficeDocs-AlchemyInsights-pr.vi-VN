---
title: Hành vi ConsistencyGuid / sourceAnchor
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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044363"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Hành vi ConsistencyGuid / sourceAnchor

Azure AD Kết nối (phiên bản 1.1.524.0 và các phiên bản sau) giờ đây hỗ trợ sử dụng msDS-ConsistencyGuid làm thuộc tính sourceAnchor. Khi sử dụng tính năng này, Azure AD Kết nối động đặt cấu hình các quy tắc đồng bộ thành:
  
- Sử dụng msDS-ConsistencyGuid làm thuộc tính sourceAnchor cho các đối tượng Người dùng. ObjectGUID được dùng cho các loại đối tượng khác.
    
- Đối với mọi đối tượng Người dùng AD tại chỗ được cung cấp có thuộc tính msDS-ConsistencyGuid không được cấp tự động, Azure AD Kết nối sẽ ghi lại giá trị OBJECTGUID vào thuộc tính msDS-ConsistencyGuid trong Active Directory tại chỗ. Sau khi thuộc tính msDS-ConsistencyGuid được nhập tự động, Azure AD Kết nối sau đó sẽ xuất đối tượng sang Azure AD.
    
 **Lưu ý:** Sau khi nhập một đối tượng AD tại chỗ vào Azure AD Kết nối (tức là, được nhập vào Không gian Trình kết nối AD và được chiếu vào Metaverse), bạn không thể thay đổi giá trị SourceAnchor của đối tượng nữa. Để chỉ định giá trị sourceAnchor cho đối tượng AD tại chỗ đã cho, hãy đặt cấu hình thuộc tính msDS-ConsistencyGuid trước khi được nhập vào Azure AD Kết nối. 
  
Để biết thêm thông tin về SourceAnchor và ConsistencyGuid, hãy tham khảo: [Azure AD Kết nối: Khái niệm thiết kế](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

