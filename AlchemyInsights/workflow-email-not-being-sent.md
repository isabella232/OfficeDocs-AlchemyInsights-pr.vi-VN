---
title: Luồng công việc email không được gửi
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766155"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Luồng công việc email không được gửi cho một danh sách SharePoint hoặc thư viện

1. Email từ luồng công việc không được gửi đến tất cả người dùng hoặc chỉ người dùng cụ thể hoặc bạn thấy lỗi **thư email không được gửi. Đảm bảo rằng e-mail có người nhận hợp lệ**.

    Kiểm tra xem người dùng tồn tại trong **tất cả mọi người** quyền nhóm (danh sách thông tin người dùng) cho bộ sưu tập trang web đó.  Mẫu URL trực tiếp:<tenant>https://.<sitename>SharePoint.com/Sites//_layouts/15/nhân .aspx? MembershipGroupId = 0

    - Nếu người dùng không tồn tại, đảm bảo rằng người dùng được đăng nhập vào trang. 
    - Nếu đó là người dùng bên ngoài, hãy đảm bảo rằng lời mời của họ đã được chấp nhận.
    - Nếu người dùng tồn tại trong nhóm quyền, đảm bảo rằng địa chỉ email là chính xác.
    - Nếu địa chỉ email của người dùng không được đặt ở đây, sau đó tạo một cảnh báo mẫu cho người dùng đó buộc đồng bộ hoá tài khoản người dùng từ hồ sơ người dùng của SharePoint vào bộ sưu tập trang web này.
 
2. Email từ luồng công việc được gửi đến quản trị viên bộ sưu tập trang web nhưng không cho người dùng khác và xem lỗi **http bị cấm <span>https:</span>//URL/_vti_bin/client.xvc.SP.Utilities.Utility.sendemail**.
 

    Xem [truy cập bị từ chối khi bạn gửi một email đến một nhóm SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Ngoài ra, xác minh rằng tính năng bộ sưu tập trang web **chế độ khoá truy cập giới hạn cho phép người dùng** không hoạt động.


## <a name="related-topics"></a>Chủ đề liên quan
Bạn muốn thử Microsoft Flow trong SharePoint Online?
- [Tạo Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint và Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


