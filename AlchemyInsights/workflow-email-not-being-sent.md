---
title: Email dòng công việc không được gửi đi
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
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749031"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Email dòng công việc không được gửi cho một danh sách hoặc thư viện SharePoint

1. Email từ dòng công việc không được gửi đến tất cả người dùng hoặc chỉ những người dùng cụ thể hoặc bạn thấy **thông báo lỗi email không thể gửi được. Hãy đảm bảo email có một người nhận hợp lệ**.

    Kiểm tra xem người dùng có tồn tại trong nhóm quyền **tất cả mọi người** (danh sách thông tin người dùng) cho tuyển tập trang đó hay không.  URL trực tiếp mẫu: https:// <tenant> . SharePoint.com/Sites/ <sitename> /_layouts/15/người. aspx? MembershipGroupId = 0

    - Nếu người dùng không tồn tại, hãy đảm bảo rằng người dùng đã đăng nhập vào trang. 
    - Nếu đó là một người dùng bên ngoài, hãy đảm bảo rằng lời mời của họ đã được chấp nhận.
    - Nếu người dùng không tồn tại trong nhóm quyền, hãy đảm bảo rằng địa chỉ email chính xác.
    - Nếu địa chỉ email của người dùng không được đặt ở đây, sau đó tạo một cảnh báo mẫu cho người dùng đó lực lượng đồng bộ của tài khoản người dùng đó từ hồ sơ người dùng của SharePoint vào tuyển tập trang này.
 
2. Email từ dòng công việc được gửi đến người quản trị tuyển tập trang nhưng không cho người dùng khác và xem lỗi **http đã cấm cho <span>https:</span>//url/_vti_bin/client.xvc.SP.Utilities.Utility.sendemail**.
 

    Xem [Access bị từ chối khi bạn gửi email đến một nhóm SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Ngoài ra, hãy xác minh rằng tính năng của bộ sưu tập trang **chế độ có quyền hạn chế của người dùng truy nhập** không hiện hoạt.


## <a name="related-topics"></a>Chủ đề liên quan
Bạn muốn thử Microsoft Flow trong SharePoint Online?
- [Tạo dòng](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint và dòng](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


