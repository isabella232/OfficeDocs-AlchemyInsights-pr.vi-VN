---
title: Tạo site trong SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732304"
---
# <a name="create-sharepoint-sites-using-templates"></a>Tạo các trang SharePoint bằng mẫu

Khả năng lưu site dưới dạng mẫu không được hỗ trợ với liên lạc hiện đại hoặc các site nhóm. Để biết thêm thông tin về cách sử dụng mẫu [, hãy tải xuống và tải lên một site SharePoint dưới dạng mẫu](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Dưới đây là một số vấn đề/giải pháp thông thường liên quan đến việc lưu một trang hoặc danh sách dưới dạng mẫu trong SharePoint Online. 

**Nút lưu site/danh sách không sẵn dùng hoặc bị thiếu**

Người quản trị sẽ cần cho phép các tập lệnh tùy chỉnh cho phép các tính năng mẫu. Để biết các bước chi tiết, ví dụ và cân nhắc 

- [Cho phép hoặc ngăn chặn các tập lệnh tùy chỉnh](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Lệnh lưu dưới dạng mẫu không được hỗ trợ và có thể gây ra sự cố trên các trang sử dụng cơ sở hạ tầng phát hành SharePoint Server.

**Không tạo được mẫu site hoặc không hoạt động đúng cách**

Mẫu có thể bị thiếu một [tính năng](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) và sẽ không kích hoạt. Nếu tính năng này không sẵn dùng để kích hoạt trong tuyển tập trang hiện tại, bạn không thể sử dụng mẫu site để tạo một site.

- Kiểm tra xem liệu có bất kỳ danh sách hay thư viện vượt quá [giới hạn dạng xem danh sách](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) của các mục 5000 khi điều này có thể chặn việc tạo một mẫu site hay không.

- Site có thể đang sử dụng quá nhiều tài nguyên và do đó mẫu site vượt quá giới hạn 50 MB.


- Có sự cố khi hiển thị dữ liệu từ danh sách sử dụng cột tra cứu. Để biết thêm thông tin, hãy xem [danh sách tạo mẫu không hiển thị dữ liệu từ danh sách tra cứu chính xác trong SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Để biết thêm thông tin chi tiết về các sự cố và giải pháp phổ biến, vui lòng kiểm tra [tạo và sử dụng mẫu site](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



