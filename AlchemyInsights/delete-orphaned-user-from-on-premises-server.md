---
title: Xóa người dùng có mồ côi khỏi máy chủ tại cơ sở
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: a6af617fa4235868f0754ff4c06f4cc73b1700ef14ea449dd1886ab100ddd384
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102296"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Xóa người dùng có mồ côi khỏi máy chủ tại cơ sở

Để loại bỏ người dùng có mồ côi, hãy làm theo các bước sau:

1. Buộc đồng bộ hóa thư mục bằng cách làm theo hướng dẫn [trong Định danh kết hợp với Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Để xác minh đồng bộ hóa thư mục, hãy [xem Định danh kết hợp với Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Nếu đồng bộ hoạt động chính xác nhưng việc xóa đối tượng Active Directory không phát sinh đến Azure AD, hãy loại bỏ đối tượng mồ côi theo cách thủ công bằng cách sử dụng một trong các lệnh ghép ngắn Azure Active Directory Module sau đây cho các lệnh ghép ngắn Windows PowerShell:

    Remove-MsolContact  
    Remove-MsolGroup  
    Remove-MsolUser

    Ví dụ, để loại bỏ ID người dùng có mồ côi john.smith@contoso.com, vốn được tạo ra bằng cách dùng đồng bộ hóa thư mục, hãy chạy lệnh ghép ngắn:

    Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com