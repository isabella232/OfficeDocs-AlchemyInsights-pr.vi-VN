---
title: Teams bổ trợ dành cho máy Mac
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
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582092"
---
# <a name="teams-add-in-for-mac"></a>Teams bổ trợ dành cho máy Mac

Để khắc phục sự cố bổ trợ Teams dành cho người dùng hệ điều hành Mac bị thiếu, hãy làm theo các bước sau:

**Bước 1:** Nếu bạn có tùy chọn Kết hợp Exchange tại chỗ (2016 CU3 trở lên), hãy sử dụng công cụ Test-HMA.ps1 để xác nhận rằng Xác thực Hiện đại Kết hợp được đặt cấu hình đúng cách. Để biết thêm thông tin, xem mục Xác thực Xác thực Hiện đại Kết hợp [cho Outlook cho iOS và Android.](https://aka.ms/TestHMAEAS)  

**Lưu ý** Sử dụng định dạng địa chỉ UPN (ví dụ: [username@contoso.com](mailto:username@contoso.com)), không phải tên miền\tên người dùng. Thực hiện việc này ngay cả đối với người Exchange Online thư của họ.

**Bước 2:** Để người dùng đi tới Tài **khoản**  >  **Công cụ**... trong Outlook for Mac và tìm và chọn tài khoản. Xác nhận tên người dùng được liệt kê có định dạng UPN (ví [dụ: username@contoso.com).](mailto:username@contoso.com)

**Bước 3:** Xác nhận người dùng đã được cấp phép Microsoft Teams dùng. Người dùng phải đang sử dụng đăng ký Office 365 cho máy Mac, phiên bản sản phẩm 16.24 trở lên.