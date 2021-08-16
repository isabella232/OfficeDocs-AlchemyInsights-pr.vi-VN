---
title: Email dòng công việc không được gửi
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072542"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Email dòng công việc không được gửi cho danh sách SharePoint thư viện

1. Email từ dòng công việc không được gửi đến tất cả người dùng hoặc chỉ những người dùng cụ thể, hoặc bạn gặp lỗi Không thể gửi thông điệp email. Đảm bảo email có người nhận **hợp lệ.**

    Kiểm tra xem người dùng có tồn tại trong nhóm **quyền Tất cả Mọi người** (danh sách thông tin người dùng) cho tuyển tập site đó không.  URL trực tiếp mẫu: <tenant> https://.sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Nếu người dùng không tồn tại, hãy đảm bảo người dùng đã đăng nhập vào trang. 
    - Nếu đó là người dùng bên ngoài, hãy đảm bảo rằng lời mời của họ đã được chấp nhận.
    - Nếu người dùng tồn tại trong nhóm quyền, hãy đảm bảo rằng địa chỉ email là chính xác.
    - Nếu địa chỉ email người dùng không được đặt ở đây, hãy tạo một cảnh báo mẫu cho người dùng đó buộc phải đồng bộ tài khoản người dùng đó từ Hồ sơ Người SharePoint vào tuyển tập site này.
 
2. Email từ dòng công việc được gửi tới người quản trị tuyển tập site nhưng không gửi đến người dùng khác và thấy lỗi HTTP Bị cấm **<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail.**
 

    Hãy [xem truy nhập bị từ chối khi bạn gửi email đến một SharePoint mới.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    Ngoài ra, xác nhận rằng tính **năng tuyển tập** site chế độ khóa quyền người dùng truy nhập hạn chế không hiện hoạt.


## <a name="related-topics"></a>Chủ đề liên quan
Bạn muốn thử Microsoft Flow thực hiện SharePoint Online?
- [Tạo Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint và Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


