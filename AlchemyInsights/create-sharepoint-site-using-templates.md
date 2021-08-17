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
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057988"
---
# <a name="create-sharepoint-sites-using-templates"></a>Tạo SharePoint site bằng cách sử dụng mẫu

Khả năng lưu site dưới dạng mẫu không được hỗ trợ với Liên lạc hoặc Site Nhóm hiện đại. Để biết thêm thông tin về cách sử dụng [mẫu, hãy xem mục Lưu, tải xuống và tải SharePoint site dưới dạng mẫu.](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)

Dưới đây là một số sự cố/giải pháp phổ biến về việc Lưu Site hoặc Danh sách dưới dạng mẫu trong Sharepoint Online. 

**Nút Lưu mẫu danh sách/site không sẵn dùng hoặc bị thiếu**

Người quản trị sẽ cần Cho phép Script Tùy chỉnh bật các tính năng của mẫu. Để biết các bước chi tiết, ví dụ và cân nhắc, hãy xem 

- [Cho phép hoặc ngăn chặn tập lệnh tùy chỉnh](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Lệnh Lưu site dưới dạng mẫu không được hỗ trợ và có thể gây ra nhiều vấn đề trên các site sử dụng Cơ sở SharePoint sở hạ tầng Phát hành Server.

**Không tạo được mẫu site hoặc không hoạt động đúng cách**

Mẫu có thể thiếu một tính [năng và](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) sẽ không kích hoạt. Nếu tính năng này không sẵn dùng để kích hoạt trong tuyển tập site hiện tại, bạn không thể dùng mẫu site để tạo một site.

- Kiểm tra xem liệu có [](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) bất kỳ danh sách hoặc thư viện nào vượt quá Ngưỡng Giới hạn Dạng xem Danh sách của 5000 mục khi điều này có thể chặn việc tạo một mẫu site.

- Site có thể đang sử dụng quá nhiều tài nguyên và do đó, mẫu site vượt quá giới hạn 50 MB.


- Có một số vấn đề hiển thị dữ liệu từ một danh sách có sử dụng một cột tra cứu. Để biết thêm thông tin, hãy xem mục Danh sách do mẫu tạo ra không hiển thị dữ liệu từ [danh sách tra cứu chính SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)

Để biết thêm thông tin chi tiết về các vấn đề và giải pháp thông thường, vui [lòng kiểm tra Tạo và sử dụng mẫu site.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



