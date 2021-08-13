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
ms.openlocfilehash: 70f8def2a0f3419a9aa6325e376ba52fc35ec48b61f39ede99d7e58cd6c6c464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971499"
---
# <a name="user-management-issues"></a>Các vấn đề về quản lý người dùng

**Điều gì sẽ xảy ra với người dùng được gán hiện tại cho ứng dụng nếu tôi vô hiệu hóa thuộc tính 'Cần gán người dùng' (đặt thuộc tính này thành Không)?**

Việc tắt gán người dùng **bắt buộc KHÔNG ảnh** hưởng đến người dùng hiện đang được gán. Việc vô hiệu hóa thuộc tính này sẽ chỉ cho phép tất cả người dùng truy nhập vào ứng dụng. Tất cả người dùng được liệt kê và những người dùng được gán cho nhóm trong ứng dụng sẽ vẫn hợp lệ.

- Để giới hạn ứng dụng của bạn cho một tập hợp người dùng cụ thể, hãy xem mục - Giới hạn ứng dụng Azure AD cho một [nhóm người dùng - bao Nền tảng định danh Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Để gán người dùng và nhóm, cho các ứng dụng doanh nghiệp trong Azure Active Directory (Azure AD), hoặc từ bên trong cổng thông tin Azure hoặc bằng cách sử dụng PowerShell, hãy xem mục Quản lý việc gán người dùng cho một ứng dụng [trong Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)
- Để ủy quyền tạo và quản lý Ứng dụng, hãy xem Quyền người quản trị quản lý ứng dụng [đại diện - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Ẩn các ứng dụng doanh nghiệp cụ thể khỏi** người dùng - Sử dụng các bước sau để ẩn tất cả Microsoft 365 từ **pa-nen MyApps.** Các ứng dụng sẽ vẫn hiển thị trong cổng Office 365 tin.

 1. Đăng nhập vào cổng thông tin Azure với tư cách là người quản trị toàn cầu cho thư mục của bạn. 
 2. Chọn **Azure Active Directory**. 
 3. Chọn **Người dùng**. 
 4. Chọn Cài **đặt người dùng**. 
 5. Bên dưới **Ứng dụng doanh nghiệp,** bấm **quản lý cách người dùng cuối khởi chạy và xem ứng dụng của họ.** 
 6. Đối **với Người dùng chỉ có thể Office 365 dụng trong cổng thông Office 365,** bấm **Có.** 
 7. Bấm vào **Lưu**. 
 8. Để biết thêm chi tiết, [hãy xem mục Ẩn ứng dụng Enterprise khỏi trải nghiệm của người dùng trong Azure AD | Tài liệu Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Nếu bạn cung cấp một ứng dụng Phần mềm dưới dạng Dịch vụ (SaaS) cho nhiều tổ chức, bạn có thể đặt cấu hình ứng dụng của mình để chấp nhận đăng nhập từ bất kỳ đối tượng thuê Azure Active Directory (Azure AD). Cấu hình này được gọi là "thực hiện nhiều đối tượng thuê ứng dụng của bạn". Người dùng trong bất kỳ đối tượng thuê Azure AD nào sẽ có thể đăng nhập vào ứng dụng của bạn sau khi chấp thuận sử dụng tài khoản của họ với ứng dụng của bạn. Để biết thêm thông tin, xem [mục Xây dựng các ứng dụng đăng nhập người dùng Azure AD - Nền tảng định danh Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Làm thế nào để người dùng cuối có thể truy nhập vào ứng dụng sau khi họ được gán cho ứng dụng?**

Mỗi ứng dụng trong Lưỡi ứng dụng doanh nghiệp có một liên kết cho người dùng cuối để truy nhập. Người dùng cũng có thể truy nhập ứng dụng thông **qua cổng thông tin Myapps** một cách dễ dàng.

- **Bạn muốn biết ứng dụng và loại ứng dụng đang được người dùng sử dụng?**

Bạn có thể tải xuống báo cáo đăng nhập trong vòng 30 ngày qua **từ portal.azure.com > Azure Active directory> Signins** để tải xuống> báo cáo.

- Tìm hiểu cách Cấp [cho người quản trị toàn đối tượng thuê sự đồng ý đối với một ứng dụng và](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) Đặt [cấu hình cách người dùng cuối đồng ý với ứng dụng.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)

- Tìm hiểu [cách chấp thuận hoạt động](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) và Quản lý sự đồng ý đối với các ứng [dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


