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
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "50714442"
---
# <a name="troubleshoot-group-issues"></a>Khắc phục sự cố nhóm

**Tôi cần gán một nhóm cho vai trò Azure AD**

Để gán nhóm Azure Active Directory (AD) vào vai trò Azure AD, hãy thực hiện các bước sau đây:

1. Tạo nhóm mới-để tạo nhóm mới:

    một. Đăng nhập vào Trung tâm quản trị Azure AD với người quản trị vai trò đặc quyền hoặc quyền người quản trị toàn cầu. 
    b. Chọn các nhóm > Azure Active Directory > tất cả các nhóm > nhóm mới. 
    c's. Tạo nhóm.

2. Gán vai trò cho nhóm trong khi tạo nhóm hoặc sau khi nhóm được tạo.

    một. Để gán vai trò cho nhóm tại thời điểm tạo nhóm, hãy chuyển đổi trên các vai trò chuyển đổi Azure AD có thể được gán cho nhóm và tạo nhóm.
    b. Để gán vai trò cho nhóm sau khi đã được tạo, hãy dẫn hướng đến tab vai trò được gán cho nhóm mới được tạo và gán vai trò cho nhóm.

**Tôi cần quản lý tư cách thành viên của một nhóm được gán cho vai trò Azure AD**

1. Để ngăn không cho độ cao của đặc quyền, theo mặc định, chỉ người quản trị vai trò đặc quyền và người quản trị toàn cầu có thể sửa đổi tư cách thành viên của một nhóm được gán cho vai trò. Tuy nhiên, họ có thể chọn gán chủ sở hữu cho một nhóm và đại diện cho nhiệm vụ này. Để biết thêm thông tin hãy xem, [sử dụng các nhóm đám mây để quản lý việc gán vai trò trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).
2. Đối với các câu hỏi thường gặp và mẹo khắc phục sự cố gán vai trò cho các nhóm trong Azure AD, hãy xem các [vai trò khắc phục sự cố được gán cho nhóm điện toán đám mây](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).

**Nhóm động**

1. Nếu bạn không thể tìm thấy thuộc tính người dùng tích hợp sẵn, hãy đảm bảo rằng thuộc tính nằm trong danh sách các thuộc tính được hỗ trợ.
2. Nếu bạn đang tìm kiếm các thuộc tính thiết bị tích hợp sẵn, hãy đảm bảo rằng thuộc tính nằm trong danh sách thuộc tính của thiết bị 
3. Ngoài các thuộc tính người dùng và thiết bị tích hợp sẵn, bạn cũng có thể sử dụng [thuộc tính phần mở rộng](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties). Sau khi đồng bộ hóa các thuộc tính của phần mở rộng từ quảng cáo Windows Server tại cơ sở hoặc từ một ứng dụng SaaS được kết nối, các thuộc tính sẽ được hiển thị trong danh sách thả xuống của bộ dựng quy tắc. Có thể tìm thấy tên thuộc tính tùy chỉnh trong thư mục bằng cách truy vấn thuộc tính của người dùng bằng PowerShell và tìm kiếm tên thuộc tính. Những điều này cũng có thể sử dụng khi xây dựng các quy tắc trong cú pháp quy tắc.
4. Đảm bảo rằng đối tượng thuê của bạn có giấy phép thích hợp. Các nhóm động yêu cầu người thuê để có giấy phép Azure AD P1 Premium. Danh sách các gói giấy phép Azure AD có thể được truy nhập [tại đây](https://azure.microsoft.com/pricing/details/active-directory/). Có thể truy nhập các gói cấp phép doanh nghiệp + tính bảo mật [tại đây](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing).
5. Đảm bảo vai trò của người dùng tạo nhóm động là người quản trị toàn cầu, người quản trị InTune, người quản trị nhóm hoặc người quản trị người dùng.
6. Xin vui lòng cho phép thời gian nhóm để định cư. Tùy thuộc vào kích cỡ của đối tượng thuê của bạn, nhóm có thể mất đến 24 giờ để tổng hợp lần đầu tiên hoặc sau khi có một quy tắc thay đổi.
7. Để biết thêm thông tin, hãy xem [tạo quy tắc dựa trên thuộc tính cho tư cách thành viên nhóm động](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).

**Tôi cần xóa nhóm**

1. Nhóm có thể bị xóa khỏi thư mục bằng cách sử dụng lệnh ghép ngắn Remove-AzureADGroup trong mô-đun Azure AD PowerShell.
2. Trước khi tìm cách xóa một nhóm đã đồng bộ trong Azure AD, hãy đảm bảo rằng bạn đã xóa tất cả giấy phép đã gán để tránh lỗi.
3. Để biết thêm thông tin về việc xóa nhóm, hãy xem mục [xóa một nhóm với giấy phép đã gán](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).

**Tôi cần khôi phục nhóm đã xóa**

1. Nếu nhóm Office 365 bị xóa, chỉ có thể khôi phục được tối đa 30 ngày trước khi xóa vĩnh viễn. Sau khi bị xóa vĩnh viễn, nhóm không còn được khôi phục. Tìm hiểu thêm về việc khôi phục các nhóm [ở đây](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).
2. Chức năng này không được hỗ trợ đối với nhóm bảo mật và nhóm phân phối.
3. Đảm bảo bạn được ủy quyền để khôi phục một nhóm Office 365. Người quản trị toàn cầu, người quản trị nhóm, người quản trị tài khoản người dùng, người quản trị dịch vụ InTune, đối tác tier1 hoặc tier2 hỗ trợ và chủ sở hữu của nhóm có thể khôi phục nhóm.
4. Khi một nhóm đã bị xóa và đã khôi phục, nó được xem như một nhóm mới và đã được tự động điền theo quy tắc. Quá trình này có thể mất đến 24 giờ.
5. Để biết thêm thông tin về việc khôi phục một nhóm đã xóa, hãy xem [khôi phục nhóm Office đã xóa 365 trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Cấu hình chính sách hết hạn nhóm**

1. Chức năng này chỉ được hỗ trợ cho các nhóm Office 365, chứ không phải cho các nhóm bảo mật và nhóm phân phối không được hỗ trợ.
2. Cấu hình và sử dụng chính sách hết hạn cho các nhóm Office 365 yêu cầu giấy phép Azure AD Premium.
3. Hiện tại, chỉ có một chính sách hết hạn có thể được cấu hình cho các nhóm Office 365 trên một đối tượng thuê.
4. Chỉ có người quản trị toàn cầu, người quản trị nhóm, người quản trị người dùng và chủ sở hữu của nhóm có thể gia hạn một nhóm.
5. Nếu nhóm Office 365 hết hạn, bạn sẽ bị xóa và chỉ có thể khôi phục được tối đa 30 ngày trước khi xóa vĩnh viễn xảy ra. Sau khi bị xóa vĩnh viễn, nhóm không còn được khôi phục. Tìm hiểu thêm về việc khôi phục các nhóm [ở đây](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Gia hạn tự động dựa trên hoạt động**

Hoạt động của người dùng từ SharePoint, Outlook và nhóm có thể kích hoạt tự động gia hạn nhóm. Các hoạt động được kiểm tra tại 35 ngày trước khi nhóm hết hạn. Nếu có hoạt động trong vòng đời nhóm hiện tại, nhóm sẽ được tự động gia hạn và thông báo email sẽ không được gửi đến người sở hữu nhóm.

**Thời gian thông báo cho các nhóm đã hết hạn**

1. Thông báo email được gửi đến chủ sở hữu nhóm 365 của Office 30 ngày, 15 ngày và 1 ngày trước ngày hết hạn của nhóm.
2. Khi bạn thiết lập trước hết hạn, bất kỳ nhóm nào cũ hơn khoảng hết hạn được đặt thành 35 ngày cho đến khi hết hạn.
3. Ngày hết hạn nhóm được tính toán dựa trên ngày gia hạn của nhóm, không dựa vào ngày Cập Nhật chính sách. Nếu Cập Nhật chính sách hết hạn, ngày hết hạn sẽ không thay đổi.
4. Để biết thêm thông tin, hãy xem, [chính sách hết hạn nhóm và email gia hạn](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) và [khôi phục một nhóm đã xóa Office 365 trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Quyền tạo nhóm**

Đảm bảo rằng bạn được ủy quyền để tạo nhóm mới. Người quản trị toàn cầu có thể tắt tính năng tạo nhóm trong cổng thông tin Azure hoặc Pa-nen truy nhập. Bạn có thể cần người quản trị để tạo nhóm mới cho bạn hoặc để cung cấp cho bạn quyền thích hợp.

1. [Tạo một nhóm mới và thêm các thành viên trong Azure Portal](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Tạo nhóm trong PowerShell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Tắt tính năng tạo nhóm trong PowerShell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Quản lý những người có thể tạo nhóm trong Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Tắt thông báo chào mừng trong Office 365 qua PowerShell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Vai trò quản trị Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Quản lý quyền tạo nhóm**

1. Người quản trị toàn cầu có thể quản lý quyền tạo nhóm cho các nhóm bảo mật hoặc Office 365 được tạo trong trang Azure Portal hoặc Pa-nen truy nhập, bằng cách thiết đặt **người dùng có thể tạo nhóm bảo mật trong Azure Portals** hoặc **người dùng có thể tạo nhóm Office 365 trong Azure Portals** cài đặt trong **tất cả các nhóm > chung (thiết đặt)**.
2. Bạn cũng có thể hạn chế tạo nhóm để chọn một nhóm người dùng nếu bạn có giấy phép Azure AD P1 Premium.

**Tắt thông báo chào mừng cho các thành viên mới của một nhóm Office 365**

Thông báo chào mừng được gửi đến những người dùng được thêm vào các nhóm Office 365 có thể bị vô hiệu hóa bằng cách đặt `UnifiedGroupWelcomeMessageEnabled` thành **false** trong PowerShell. Tìm hiểu về thiết đặt này [ở đây](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).













