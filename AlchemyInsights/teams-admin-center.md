---
title: Teams Trung tâm Quản trị
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 29e54e0f8255b4ce84c433f2cc827aaedf35327626f0095788faef802763bc53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049366"
---
# <a name="teams-admin-center"></a>Teams Trung tâm Quản trị

Tìm hiểu về quản lý Teams với Trung [tâm quản Teams Chính .](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center)

Nếu bạn không thể truy nhập vào Trung tâm Quản Teams, vui lòng kiểm tra các mục sau:

- Xác minh rằng bạn đã cho phép địa chỉ [IP Office 365 và URL](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) thích hợp trên mọi thiết bị ngoại vi (tường lửa, v.v.) hoặc trong quy tắc tường lửa trên máy cục bộ của bạn.
- Xác minh rằng đăng nhập bạn đang sử dụng để truy nhập vào Cổng thông tin Quản trị Teams khớp với tên người dùng của bạn được liệt [kê trong cổng thông tin Quản trị Microsoft 365.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)

Nếu người dùng không xuất hiện trong Trung tâm Quản trị Teams, vui lòng kiểm tra như sau:

- Bạn đã tạo người dùng hoặc đã gán giấy phép trong 24 giờ qua chưa? Vui lòng đảm bảo rằng bạn chờ ít nhất 24 giờ trước khi mở một vé hỗ trợ.
- Xác minh rằng bạn đã gán giấy phép thích hợp?
- Nếu bạn có Active Directory tại cơ sở, hãy xác nhận rằng giá trị [của msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) hoặc địa chỉ SIP trong trường ProxyAddresses trong Active Directory cục bộ của bạn là duy nhất và định dạng khớp với sip: Tên người dùng của người dùng từ [Trung tâm quản trị Microsoft 365.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)
- Nếu bạn dự định duy trì triển khai Skype for Business Server và cho phép người dùng ở nhà tại chỗ và Trực tuyến: hãy theo dõi "Thiết lập kết hợp với Teams và **Skype for Business Online"** trong Panel Điều khiển Skype for Business Server và di chuyển người dùng Trực tuyến.
