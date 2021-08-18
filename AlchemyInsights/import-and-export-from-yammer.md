---
title: Nhập và xuất từ Yammer
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
ms.openlocfilehash: b365921d3ca64e8ad4bd3891e11add8043b2a903
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329848"
---
# <a name="import-and-export-from-yammer"></a>Nhập và xuất từ Yammer

**Nhập**

Các tùy chọn nhập người dùng sẽ khác nhau tùy thuộc vào việc mạng Yammer của bạn đang ở Chế độ [Gốc cho Microsoft 365,](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)hoặc không.

- **Chế độ Không** phải Dành riêng: Người dùng có thể được nhập vào các nhóm bằng cách [](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) sử dụng Thêm từ Sổ Địa chỉ [(giới](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) hạn 100 người dùng) trong thiết đặt nhóm hoặc vào mạng bằng cách sử dụng Cập nhật Hàng loạt trong Người quản trị Mạng.
- **Chế độ Gốc**: Phải thực hiện các thao tác tư cách thành viên nhóm và tư cách thành viên mạng từ cổng thông tin quản trị [Microsoft 365,](https://docs.microsoft.com/microsoft-365/admin/add-users)cổng thông tin [Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)hoặc sử dụng một tùy chọn Azure AD khác. Các mạng ở Chế độ Gốc sẽ không còn có quyền truy nhập vào Cập nhật Hàng loạt và các tính năng kế thừa khác nữa.

    **Quan trọng**: Yammer bao giờ được hỗ trợ nhập nội dung từ bên trong Người quản trị Mạng ngay cả khi tính năng Xuất Dữ liệu đã được sử dụng trong mạng khác. Nội dung có thể được đăng lại bởi các giải pháp đối tác hoặc API REST Yammer lại.

**Xuất**

[Xuất Dữ liệu Mạng trong Người quản trị Mạng](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) cho phép xuất nội dung từ Yammer mạng khác, bao gồm tin nhắn và tệp. Tệp đính kèm có thể cực lớn và sẽ khiến cho hoạt động xuất mất nhiều thời gian hoàn thành. Chúng tôi khuyên bạn nên xuất các mạng hiện hoạt bằng [CÁCH sử dụng API](https://developer.yammer.com/docs/data-export-api) Xuất Dữ liệu theo các khối theo ngày hoặc tuần. Bộ trợ giúp của Microsoft không cung cấp tập lệnh tùy chỉnh cho mục đích này.

Đã tồn tại [xuất GDPR riêng](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) biệt để xuất nội dung cho một người dùng cá nhân.