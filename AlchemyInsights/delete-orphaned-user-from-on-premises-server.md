---
title: Xoá người dùng đơn lẻ từ máy chủ tại chỗ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198582"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Xoá người dùng đơn lẻ từ máy chủ tại chỗ

Để loại bỏ người dùng đơn lẻ, hãy làm theo các bước sau:

1. Áp dụng đồng bộ hóa thư mục bằng cách làm theo hướng dẫn trong [danh tính lai với Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Để xác minh đồng bộ hóa thư mục, xem [danh tính lai với Azure Active Directory là gì?](https://technet.microsoft.com/library/jj151797.aspx).

3. Nếu đồng bộ hoá chức năng chính xác nhưng xoá đối tượng Active Directory không tuyên truyền Azure AD, xoá thủ công các đối tượng đơn lẻ bằng cách sử dụng một trong các lệnh ghép ngắn Azure Active Directory mô-đun Windows PowerShell:

    Loại bỏ-MsolContact  
    Loại bỏ-MsolGroup  
    Loại bỏ-MsolUser

    Ví dụ: để loại bỏ người dùng đơn lẻ ID john.smith@contoso.com, ban đầu được tạo ra bằng cách sử dụng đồng bộ hóa thư mục, chạy lệnh:

    Loại bỏ-MsolUser-UserPrincipalName John.Smith@Contoso.com