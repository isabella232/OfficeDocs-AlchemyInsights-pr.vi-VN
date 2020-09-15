---
title: Bổ trợ nhóm cho Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670350"
---
# <a name="teams-add-in-for-mac"></a>Bổ trợ nhóm cho Mac

Để khắc phục sự cố dành cho các bổ trợ nhóm không bị thiếu cho người dùng hệ điều hành Mac, hãy làm theo các bước sau đây:

**Bước 1:** Nếu bạn có kết hợp Exchange tại cơ sở (2016 CU3 hoặc phiên bản mới hơn), hãy sử dụng công cụ Test-HMA.ps1 để xác nhận rằng kết hợp xác thực hiện đại sẽ được cấu hình đúng. Để biết thêm thông tin, hãy xem mục [phê chuẩn thiết lập xác thực hiện đại cho Outlook for iOS và Android](https://aka.ms/AA980zq).  

**Ghi chú** Sử dụng định dạng địa chỉ UPN (ví dụ, [username@contoso.com](mailto:username@contoso.com)), không phải là \ tên người dùng. Hãy làm điều này ngay cả đối với người dùng với hộp thư Exchange Online.

**Bước 2:** Người dùng đã đi đến **Tools**các  >  **tài khoản**công cụ... trong Outlook for Mac, và tìm và chọn tài khoản. Xác nhận tên người dùng được liệt kê ở định dạng UPN (ví dụ, [username@contoso.com](mailto:username@contoso.com)).

**Bước 3:** Xác nhận người dùng là người dùng Microsoft nhóm được cấp phép. Người dùng phải sử dụng đăng ký Office 365 cho máy Mac, phiên bản sản phẩm 16,24 hoặc mới hơn.