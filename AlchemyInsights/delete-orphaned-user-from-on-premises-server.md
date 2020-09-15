---
title: Xóa người dùng mồ côi từ máy chủ tại cơ sở
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
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680157"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Xóa người dùng mồ côi từ máy chủ tại cơ sở

Để loại bỏ một người dùng mồ côi, hãy làm theo các bước sau đây:

1. Đồng bộ hóa Directory bằng cách làm theo các hướng dẫn trong [danh tính hỗn hợp với Azure Active Directory là gì?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Để xác minh việc đồng bộ hóa thư mục, hãy xem [danh tính kết hợp với Azure Active Directory là gì?](https://technet.microsoft.com/library/jj151797.aspx).

3. Nếu các hàm đồng bộ chính xác nhưng việc xóa đối tượng Active Directory không được tuyên truyền với Azure AD, hãy loại bỏ các đối tượng mồ côi bằng cách dùng một trong các lệnh ghép ngắn Azure Active Directory cho Windows PowerShell:

    Loại bỏ-MsolContact  
    Loại bỏ-MsolGroup  
    Loại bỏ-MsolUser

    Ví dụ: để loại bỏ người dùng mồ côi ID john.smith@contoso.com, ban đầu được tạo bằng cách sử dụng đồng bộ hóa thư mục, hãy chạy lệnh ghép ngắn:

    Loại bỏ-MsolUser – UserPrincipalName John.Smith@Contoso.com