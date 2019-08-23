---
title: Quy trình làm việc email chưa được gửi
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530913"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Quy trình làm việc email chưa được gửi cho một danh sách SharePoint hoặc thư viện

1. Email từ quy trình công việc sẽ không được gửi đến tất cả người dùng hoặc chỉ có người dùng cụ thể, hoặc bạn nhìn thấy các lỗi **thư e-mail không thể gửi. Đảm bảo rằng e-mail đã nhận hợp lệ**.

    Kiểm tra nếu người dùng tồn tại trong **Tất cả mọi người** quyền nhóm (danh sách thông tin người dùng) cho rằng bộ sưu tập trang web.  Mẫu trực tiếp URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Nếu người dùng không tồn tại, đảm bảo rằng người dùng được đăng nhập vào trang. 
    - Nếu nó là một người dùng bên ngoài, đảm bảo rằng lời mời của họ đã được chấp nhận.
    - Nếu người dùng không tồn tại trong nhóm quyền, đảm bảo rằng địa chỉ email là chính xác.
    - Nếu địa chỉ email mà người dùng không được thiết lập ở đây, sau đó tạo ra một cảnh báo mẫu cho người dùng đó mà các lực lượng đồng bộ của tài khoản người dùng đó từ hồ sơ người dùng SharePoint bộ sưu tập trang web này.
 
2. Email từ quy trình công việc sẽ được gửi đến người quản trị bộ sưu tập trang web, nhưng không cho người dùng khác và xem lỗi **HTTP Cấm để <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Xem [Truy cập từ chối khi bạn gửi một email cho một nhóm SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Ngoài ra, xác minh rằng không phải là tính năng bộ sưu tập trang web của **chế độ khoá cứng hạn chế truy cập người dùng cho phép** hoạt động.


## <a name="related-topics"></a>Chủ đề liên quan
Bạn muốn thử Microsoft Flow trong SharePoint Online?
- [Tạo ra dòng chảy](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint và dòng chảy](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


