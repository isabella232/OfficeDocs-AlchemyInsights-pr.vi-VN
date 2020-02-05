---
title: Tạo một trang web trong SharePoint trực tuyến
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770445"
---
# <a name="create-sharepoint-sites-using-templates"></a>Tạo các trang web SharePoint bằng cách sử dụng mẫu

Khả năng lưu một trang web như là một mẫu không được hỗ trợ với giao tiếp hiện đại hoặc nhóm Sites. Để biết thêm thông tin về cách sử dụng mẫu [, xem lưu, tải xuống và tải lên trang web SharePoint làm mẫu](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Dưới đây là một số vấn đề thường gặp/giải pháp liên quan đến lưu một trang web hoặc danh sách như một mẫu trong SharePoint Online. 

**Lưu trang web/danh sách mẫu nút không có sẵn hoặc thiếu**

Quản trị viên sẽ cần cho phép tuỳ chỉnh script để kích hoạt các tính năng mẫu. Để biết các bước chi tiết, ví dụ và xem xét 

- [Cho phép hoặc ngăn chặn tập lệnh tùy chỉnh](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Lưu trang web dưới dạng lệnh không được hỗ trợ và có thể gây ra sự cố trên các trang web sử dụng SharePoint Server xuất bản cơ sở hạ tầng.

**Mẫu trang web không thể tạo hoặc không hoạt động bình thường**

Mẫu có thể thiếu một [tính năng](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) và sẽ không kích hoạt. Nếu tính năng không có sẵn để kích hoạt trong bộ sưu tập trang web hiện tại, bạn không thể sử dụng mẫu trang web để tạo một trang web.

- Kiểm tra xem nếu có danh sách hoặc thư viện vượt quá [ngưỡng giới hạn xem danh sách](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 mục vì điều này có thể chặn tạo một mẫu trang web.

- Trang web có thể sử dụng quá nhiều tài nguyên và do đó các trang web mẫu vượt quá giới hạn 50 MB.


- Có vấn đề Hiển thị dữ liệu từ danh sách sử dụng cột tìm kiếm. Để biết thêm thông tin, hãy xem [danh sách tạo mẫu không hiển thị dữ liệu từ danh sách tìm kiếm chính xác trong SharePoint trực tuyến](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Để biết thêm thông tin về các vấn đề và giải pháp phổ biến, hãy kiểm tra [tạo và sử dụng các mẫu trang web](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



