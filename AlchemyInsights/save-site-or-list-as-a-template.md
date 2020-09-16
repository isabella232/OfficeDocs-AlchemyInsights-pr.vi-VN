---
title: Lưu site hoặc danh sách dưới dạng mẫu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727553"
---
# <a name="save-site-or-list-as-a-template"></a>Lưu site hoặc danh sách dưới dạng mẫu

Các mẫu site SharePoint là các định nghĩa được thiết kế sẵn xung quanh một nhu cầu doanh nghiệp cụ thể. Để biết thêm thông tin, hãy xem [sử dụng mẫu để tạo các loại site SharePoint khác nhau](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Dưới đây là một số vấn đề/giải pháp thông thường liên quan đến việc lưu một trang hoặc danh sách dưới dạng mẫu trong SharePoint Online.

**Nút lưu site/danh sách không sẵn dùng hoặc bị thiếu**. 

- Người quản trị sẽ cần cho phép các tập lệnh tùy chỉnh cho phép các tính năng mẫu. Để biết các bước chi tiết, ví dụ và cân nhắc xem [cho phép hoặc ngăn chặn các kịch bản tùy chỉnh](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Lệnh lưu dưới dạng mẫu không được hỗ trợ và có thể gây ra sự cố trên các trang sử dụng cơ sở hạ tầng phát hành SharePoint Server.


**Không tạo được mẫu site hoặc không hoạt động đúng cách**

- Mẫu có thể bị thiếu một [tính năng](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) và sẽ không kích hoạt. Nếu tính năng này không sẵn dùng để kích hoạt trong tuyển tập trang hiện tại, bạn không thể sử dụng mẫu site để tạo một site.


- Kiểm tra xem liệu có bất kỳ danh sách hay thư viện vượt quá [giới hạn dạng xem danh sách](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) của các mục 5000 khi điều này có thể chặn việc tạo một mẫu site hay không.


- Site có thể đang sử dụng quá nhiều tài nguyên và do đó mẫu site vượt quá giới hạn megabyte (MB) 50.


- Có sự cố khi hiển thị dữ liệu từ danh sách sử dụng cột tra cứu. Để biết thêm thông tin, hãy xem [danh sách tạo mẫu không hiển thị dữ liệu từ danh sách tra cứu chính xác trong SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Để biết thêm thông tin chi tiết về các sự cố và giải pháp thông thường, vui lòng tham khảo, [tạo và sử dụng mẫu site](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

