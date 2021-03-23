---
title: Nhập và xuất từ yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037253"
---
# <a name="import-and-export-from-yammer"></a>Nhập và xuất từ yammer

**Xuất**

Các tùy chọn nhập người dùng khác nhau tùy thuộc vào việc mạng yammer của bạn nằm trong [chế độ bản địa cho Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)hay không.

- **Chế độ không phải là bản địa**: người dùng có thể được nhập vào các nhóm bằng cách dùng [Thêm từ sổ địa chỉ](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (giới hạn đối với người dùng 100) trong thiết đặt nhóm hoặc vào mạng bằng cách dùng [Cập nhật hàng loạt](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) trong quản trị mạng.
- **Chế độ bản địa**: thành viên nhóm và các hoạt động thành viên mạng phải được thực hiện từ [cổng thông tin quản trị Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [cổng thông tin Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)hoặc dùng tùy chọn Azure AD khác. Các mạng trong chế độ bản địa không còn có quyền truy nhập vào bản cập nhật hàng loạt và các tính năng kế thừa khác.

> [!IMPORTANT]
> Yammer không bao giờ được hỗ trợ nhập nội dung từ bên trong quản trị mạng ngay cả khi tính năng xuất dữ liệu được sử dụng trong một mạng khác. Nội dung có thể được đăng lên bởi các giải pháp đối tác hoặc các API trong phần còn lại của yammer.

**Ngạch**

[Xuất dữ liệu mạng trong quản trị mạng](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) cho phép xuất nội dung từ mạng yammer, bao gồm các thư và tệp. Tệp đính kèm có thể rất lớn và sẽ gây ra xuất khẩu để có thời gian đáng kể để hoàn thành. Chúng tôi khuyên bạn nên xuất các mạng hiện hoạt bằng cách dùng [API xuất dữ liệu](https://developer.yammer.com/docs/data-export-api) trong chunks theo ngày hoặc tuần. Hỗ trợ của Microsoft sẽ không cung cấp các tập lệnh tùy chỉnh cho mục đích này.

Xuất một [Gdpr](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) riêng biệt tồn tại để xuất nội dung cho một người dùng cá nhân.