---
title: Khắc phục sự cố nhóm
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 47f00118a5a4b446b6a3b06f0fc6101d00d11b626eaf249bb6ca962a55f7f4d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939365"
---
# <a name="troubleshoot-group-issues"></a>Khắc phục sự cố nhóm

**Tôi cần gán nhóm cho vai trò Azure AD**

Để gán một nhóm Azure Active Directory quyền (AD) cho vai trò Azure AD, hãy thực hiện các bước sau đây:

1. Tạo nhóm mới - Để tạo một nhóm mới:

    a. Đăng nhập vào trung tâm quản trị Azure AD với người quản trị vai trò đặc quyền hoặc quyền của người quản trị toàn cầu. 
    b. Chọn Azure Active Directory > Nhóm > nhóm Tất cả > Nhóm mới. 
    c. Tạo nhóm.

2. Gán vai trò cho nhóm trong quá trình tạo nhóm hoặc sau khi tạo nhóm.

    a. Để gán vai trò cho nhóm vào lúc tạo nhóm, bạn có thể bật nút bật tắt vai trò Azure AD cho nhóm, rồi tạo nhóm.
    b. Để gán vai trò cho nhóm sau khi tạo nhóm, dẫn hướng đến tab Vai trò được gán cho nhóm mới được tạo, rồi gán vai trò cho nhóm đó.

**Tôi cần quản lý tư cách thành viên của nhóm được gán vai trò Azure AD**

1. Để ngăn mức nâng cao đặc quyền, theo mặc định, chỉ người quản trị vai trò có đặc quyền và người quản trị toàn cầu mới có thể sửa đổi tư cách thành viên của nhóm được gán vai trò. Tuy nhiên, họ có thể chọn giao chủ sở hữu cho một nhóm như vậy và ủy nhiệm nhiệm vụ này. Để biết thêm thông tin, hãy [xem mục Sử dụng nhóm đám mây để quản lý việc gán vai trò Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)
2. Để biết các câu hỏi thường gặp và mẹo khắc phục sự cố về gán vai trò cho các nhóm trong Azure AD, hãy xem mục Khắc phục sự cố vai trò [được gán cho nhóm điện toán đám mây](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).

**Nhóm động**

1. Nếu bạn không thể tìm thấy các thuộc tính người dùng dựng sẵn, hãy đảm bảo rằng thuộc tính có trong danh sách các thuộc tính được hỗ trợ.
2. Nếu bạn đang tìm kiếm thuộc tính thiết bị tích hợp sẵn, hãy đảm bảo rằng thuộc tính có trong danh sách thuộc tính thiết bị 
3. Ngoài các thuộc tính thiết bị và người dùng tích hợp sẵn, bạn cũng có thể sử dụng Thuộc [tính Phần mở rộng.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties) Sau khi đồng bộ các thuộc tính phần mở rộng từ Windows Server AD tại chỗ hoặc từ ứng dụng SaaS được kết nối, các thuộc tính sẽ hiển thị trong danh sách thả xuống của bộ dựng quy tắc. The custom attribute name can be found in the directory by querying a user's attribute using PowerShell and searching for the attribute name. Các quy tắc này cũng có thể được sử dụng khi xây dựng quy tắc trong cú pháp quy tắc.
4. Đảm bảo rằng đối tượng thuê của bạn có giấy phép thích hợp. Nhóm động yêu cầu đối tượng thuê phải có giấy phép Azure AD P1 Premium động. Bạn có thể truy nhập danh sách các gói giấy phép Azure AD tại [đây.](https://azure.microsoft.com/pricing/details/active-directory/) Enterprise Mobility + Security licensing plans can be accessed [here](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing).
5. Đảm bảo rằng vai trò của người dùng khi tạo nhóm động là người quản trị toàn cầu, người quản trị intune, người quản trị nhóm hoặc người quản trị người dùng.
6. Vui lòng cho phép nhóm đến đây. Tùy theo kích cỡ đối tượng thuê của bạn, nhóm có thể mất đến 24 giờ để dân số lần đầu tiên hoặc sau khi quy tắc thay đổi.
7. Để biết thêm thông tin, hãy [xem tạo quy tắc dựa trên thuộc tính cho tư cách thành viên nhóm động.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership)

**Tôi cần xóa nhóm**

1. Các nhóm có thể bị xóa khỏi thư mục bằng cách sử dụng lệnh ghép ngắn Remove-AzureADGroup nhóm trong mô-đun Azure AD Powershell.
2. Trước khi tìm cách xóa nhóm được đồng bộ trong Azure AD, hãy đảm bảo bạn đã xóa mọi giấy phép đã gán để tránh lỗi.
3. Để biết thêm thông tin về việc xóa nhóm, [hãy xem mục Xóa nhóm có giấy phép đã gán](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).

**Tôi cần khôi phục nhóm đã xóa**

1. Nếu xóa Office 365 người dùng, bạn chỉ có thể khôi phục nhóm đó tối đa 30 ngày trước khi thực hiện xóa vĩnh viễn. Sau khi đã xóa vĩnh viễn, nhóm sẽ không còn được khôi phục. Tìm hiểu thêm về việc khôi phục nhóm [tại đây](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).
2. Chức năng này không được hỗ trợ cho nhóm bảo mật và nhóm phân phối.
3. Đảm bảo bạn được phép khôi phục nhóm Office 365 Người dùng. Người quản trị toàn cầu, người quản trị nhóm, người quản trị tài khoản người dùng, người quản trị dịch vụ intune, hỗ trợ đối tác cấp 1 hoặc lớp 2 và chủ sở hữu của nhóm có thể khôi phục nhóm.
4. Khi một nhóm động bị xóa và khôi phục, nhóm đó sẽ được xem như là một nhóm mới và được cấp lại theo quy tắc. Quy trình này có thể mất đến 24 giờ.
5. Để biết thêm thông tin về việc khôi phục nhóm đã xóa, hãy xem Khôi [phục nhóm Office 365 đã xóa Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Cấu hình chính sách hết hạn nhóm**

1. Chức năng này chỉ được hỗ trợ Office 365 nhóm người dùng và không hỗ trợ cho nhóm bảo mật và nhóm phân phối.
2. Việc đặt cấu hình và sử dụng chính sách hết hạn cho Office 365 thể yêu cầu giấy phép Azure AD Premium hạn.
3. Hiện tại, chỉ có thể cấu hình một chính sách hết hạn cho Office 365 của đối tượng thuê.
4. Chỉ người quản trị Toàn cầu, người quản trị nhóm, người quản trị người dùng và chủ sở hữu của nhóm mới có thể gia hạn nhóm.
5. Nếu một Office 365 nhóm đã hết hạn, nhóm đó sẽ bị xóa và chỉ có thể khôi phục tối đa 30 ngày trước khi xảy ra xóa vĩnh viễn. Sau khi đã xóa vĩnh viễn, nhóm sẽ không còn được khôi phục. Tìm hiểu thêm về việc khôi phục nhóm [tại đây](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Tự động gia hạn dựa trên hoạt động**

Các hoạt động người dùng từ SharePoint, Outlook và người dùng có Teams động gia hạn tự động cho nhóm. Các hoạt động được kiểm tra trong 35 ngày trước khi nhóm hết hạn. Nếu có hoạt động trong vòng đời nhóm hiện tại, nhóm đó sẽ được tự động gia hạn và thông báo qua email sẽ không được gửi đến các chủ sở hữu nhóm.

**Thời gian thông báo cho nhóm đã hết hạn**

1. Thông báo qua email được gửi Office 365 chủ nhóm 30 ngày, 15 ngày và 1 ngày trước khi hết hạn nhóm.
2. Khi bạn thiết lập hết hạn lần đầu, bất kỳ nhóm nào cũ hơn khoảng hết hạn được đặt thành 35 ngày cho đến khi hết hạn.
3. Ngày hết hạn nhóm được tính toán dựa trên ngày gia hạn của nhóm, không dựa trên ngày cập nhật chính sách. Nếu chính sách hết hạn được cập nhật, ngày hết hạn sẽ không thay đổi.
4. Để biết thêm thông tin, hãy xem mục Chính sách Hết hạn Nhóm và [email](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) gia hạn và Khôi phục Office 365 [đã xóa Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Quyền tạo nhóm**

Đảm bảo rằng bạn được phép tạo một nhóm mới. Người quản trị toàn cầu có thể tắt tính năng tạo nhóm trong cổng thông tin Azure hoặc Panel Truy nhập. Bạn có thể cần người quản trị để tạo nhóm mới cho bạn hoặc cung cấp cho bạn các quyền thích hợp.

1. [Tạo nhóm mới và thêm thành viên vào cổng thông tin Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Tạo nhóm trong Powershell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Tắt tính năng tạo nhóm trong Powershell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Quản lý những người có thể tạo nhóm trong Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Tắt thông Office 365 chào mừng qua Powershell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Vai trò quản trị Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Quản lý quyền tạo Nhóm**

1. Người quản trị toàn cầu có thể quản lý quyền tạo nhóm cho các nhóm bảo mật hoặc nhóm Office 365 được tạo trong cổng thông tin Azure hoặc Panel Truy nhập, bằng cách đặt mục Người dùng có thể tạo nhóm bảo mật trong cổng thông tin **Azure** hoặc Người dùng có thể tạo nhóm **Office 365** trong cài đặt Cổng thông tin Azure trong Tất cả các nhóm > **Chung (Cài đặt).**
2. Bạn cũng có thể hạn chế tạo nhóm để chọn nhóm người dùng nếu bạn có giấy phép Azure AD P1 Premium nhóm.

**Tắt thông báo chào mừng cho các thành viên mới của một nhóm Office 365 mới**

Thông báo chào mừng được gửi đến những người dùng được thêm vào Office 365 nhóm có thể bị vô hiệu hóa bằng cách `UnifiedGroupWelcomeMessageEnabled` **đặt thành False** trong Powershell. Tìm hiểu về cài đặt này [tại đây](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).













