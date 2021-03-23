---
title: Các vấn đề về quản lý người dùng
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037514"
---
# <a name="user-management-issues"></a>Các vấn đề về quản lý người dùng

**Điều gì xảy ra đối với người dùng hiện tại được gán cho ứng dụng nếu tôi vô hiệu hóa việc gán người dùng thuộc tính ' bắt buộc ' (đặt thuộc tính này thành không)?**

Vô hiệu hóa việc **gán yêu cầu người dùng** không ảnh hưởng đến người dùng hiện đang được gán. Việc vô hiệu hóa thuộc tính này sẽ chỉ cho phép tất cả người dùng truy nhập vào ứng dụng. Tất cả người dùng được liệt kê và những người dùng đó được gán cho các nhóm trong ứng dụng sẽ vẫn có hiệu lực.

- Để hạn chế ứng dụng của bạn cho một tập hợp người dùng cụ thể, hãy xem- [hạn chế ứng dụng AZURE AD cho một tập hợp người dùng-nền tảng Microsoft Identity | ](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.)Tài liệu Microsoft.
- Để gán người dùng và nhóm, đến các ứng dụng doanh nghiệp trong Azure Active Directory (Azure AD), từ trong cổng thông tin Azure hoặc bằng cách sử dụng PowerShell, hãy xem [quản lý việc gán người dùng cho một ứng dụng trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- Để tạo và quyền quản lý ứng dụng đại diện, hãy xem mục [quyền quản trị ứng dụng đại diện-AZURE AD | ](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles)Tài liệu Microsoft.
- **Ẩn các ứng dụng doanh nghiệp cụ thể từ người dùng** -dùng các bước sau đây để ẩn tất cả các ứng dụng Microsoft 365 từ Pa-nen **Myapps** . Các ứng dụng sẽ vẫn hiển thị trong cổng thông tin Office 365.

 1. Đăng nhập vào cổng thông tin Azure với tư cách là người quản trị toàn cầu cho thư mục của bạn. 
 2. Chọn **Azure Active Directory**. 
 3. Chọn **người dùng**. 
 4. Chọn **thiết đặt người dùng**. 
 5. Bên dưới **ứng dụng doanh nghiệp**, hãy bấm **quản lý cách người dùng cuối khởi động và xem các ứng dụng của họ**. 
 6. Đối với **người dùng chỉ có thể xem các ứng dụng office 365 trong cổng thông tin office 365**, bấm **có**. 
 7. Bấm vào **Lưu**. 
 8. Để biết thêm chi tiết, hãy xem [ẩn ứng dụng doanh nghiệp từ trải nghiệm của người dùng trong AZURE AD | ](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)Tài liệu Microsoft

- Nếu bạn cung cấp một phần mềm như một ứng dụng dịch vụ (SaaS) cho nhiều tổ chức, bạn có thể cấu hình ứng dụng của bạn để chấp nhận đăng nhập từ bất kỳ đối tượng thuê Azure Active Directory (Azure AD). Cấu hình này được gọi là "làm cho ứng dụng nhiều đối tượng thuê của bạn". Người dùng trong mọi đối tượng thuê Azure AD sẽ có thể đăng nhập vào ứng dụng của bạn sau khi đồng ý với việc sử dụng tài khoản của bạn với ứng dụng của bạn. Để biết thêm thông tin, hãy xem mục [xây dựng các ứng dụng đăng nhập vào AZURE AD users-Microsoft Identity Platform | ](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant)Tài liệu Microsoft.

- **Làm thế nào để người dùng cuối có thể truy nhập vào ứng dụng sau khi gán cho ứng dụng này?**

Mỗi ứng dụng trong lưỡi ứng dụng Enterprise đều có liên kết cho người dùng cuối truy nhập. Người dùng cũng có thể truy nhập ứng dụng thông qua cổng thông tin **Myapps** theo một cách dễ dàng.

- **Bạn muốn biết những ứng dụng và loại ứng dụng nào đang được người dùng sử dụng?**

Bạn có thể tải xuống các báo cáo đăng nhập trong vòng 30 ngày kể từ **portal.azure.com > Azure Active directory> đăng ký> báo cáo tải xuống**.

- Tìm hiểu cách [cấp sự đồng ý người quản trị toàn bộ đối tượng thuê cho một ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) và [cấu hình cách người dùng cuối đồng ý với các ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).

- Hiểu [cách đồng ý công việc](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) và [quản lý sự đồng ý với các ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


