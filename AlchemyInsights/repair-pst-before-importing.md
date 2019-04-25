---
title: Sửa chữa PST tập tin trước khi nhập khẩu
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1226
ms.assetid: ''
ms.openlocfilehash: 66b045c04ccbeb133e1bae3b9c29e01b4820d33f
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909678"
---
# <a name="repair-pst-file-before-importing"></a>Sửa chữa PST tập tin trước khi nhập khẩu

Trước khi bạn nhập một tập tin PST trong Outlook, kiểm tra các tập tin không bị hỏng bởi sửa chữa các tập tin:

1. Thoát Outlook.

2. Tìm và chạy `Scanpst.exe` trong thư mục chương trình văn phòng (C:\Program Files (x86) \Microsoft Office\root\Office\<Phiên bản\> hoặc C:\Program Files\Microsoft Office\root\Office\<Phiên bản\>).

3. Trong **Microsoft Outlook hộp thư đến sửa chữa công cụ**, hãy nhấp vào **trình duyệt** để tìm tệp .PST (ví dụ, trong C:\Users\\<username\>\AppData\Local\Microsoft\Outlook). Chọn .pst tập tin và sau đó nhấp vào **mở**.

4. Nhấp vào **bắt đầu** để bắt đầu quá trình quét.

5. Nếu phát hiện lỗi trong tập tin, nhấp vào **sửa chữa**, và sau đó nhấp vào **OK** khi sửa chữa hoàn tất.

6. Cố gắng để nhập khẩu các tập tin PST trong Outlook một lần nữa.

Để biết thêm chi tiết, xem [tập tin dữ liệu Outlook Sửa chữa](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) và [sửa chữa vấn đề nhập khẩu một tập tin PST Outlook](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).