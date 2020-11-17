---
title: Vai trò quản lý danh tính đặc quyền
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089146"
---
# <a name="privileged-identity-managementpim-role"></a>Vai trò quản lý danh tính đặc quyền (PIM)

**Quyền không được cấp sau khi kích hoạt một vai trò**

Khi bạn kích hoạt một vai trò trong Azure AD quản lý danh tính đặc quyền (PIM), kích hoạt có thể không được truyền ngay lập tức vào tất cả các cổng yêu cầu vai trò đặc quyền. Đôi khi, ngay cả khi thay đổi được tuyên truyền, bộ đệm ẩn web trong một cổng thông tin có thể dẫn đến thay đổi này không có hiệu lực ngay lập tức.

Nếu kích hoạt của bạn bị trì hoãn, hãy làm theo các bước sau đây:

1. Đăng xuất khỏi cổng thông tin Azure và sau đó đăng nhập lại. Khi bạn kích hoạt một vai trò Azure AD hoặc vai trò tài nguyên Azure, bạn sẽ thấy các giai đoạn của kích hoạt. Sau khi tất cả các giai đoạn hoàn tất, bạn sẽ thấy liên kết ' đăng xuất '. Bạn có thể sử dụng liên kết này để đăng xuất. Việc này sẽ giải quyết hầu hết các trường hợp cho việc trì hoãn kích hoạt.
2. Trong PIM, hãy xác nhận rằng bạn được liệt kê là thành viên của vai trò đó.
3. Nếu bạn đang kích hoạt vai trò người quản trị Exchange, hãy đảm bảo rằng bạn đăng xuất và đăng nhập lại. Nếu sự cố vẫn tiếp diễn, hãy mở một vé hỗ trợ và nâng cao này làm vấn đề. Nếu bạn đang sử dụng vai trò người quản trị Exchange của mình để truy nhập vào Trung tâm bảo mật và tuân thủ, hãy xem bước tiếp theo.
4. Nếu bạn đang kích hoạt một vai trò để truy nhập vào Trung tâm bảo mật và tuân thủ hoặc nếu bạn đang kích hoạt vai trò người quản trị SharePoint, bạn sẽ gặp một số trì hoãn kích hoạt từ vài phút lên đến vài giờ. Đây là một vấn đề đã biết và chúng tôi đang tích cực làm việc với các nhóm này để giải quyết sự cố này càng sớm càng tốt.

Để biết thêm thông tin, hãy xem:

- [Kích hoạt Azure AD Roles của tôi trong PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Kích hoạt các vai trò tài nguyên Azure của tôi trong PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Quyền không bị loại bỏ sau khi hủy kích hoạt một vai trò hoặc kích hoạt vai trò hết hạn**

Khi bạn hủy kích hoạt một vai trò trong quản lý căn cước có đặc quyền Azure AD hoặc khi nào hết hạn, có thể có một sự chậm trễ mà bạn tiếp tục có quyền truy nhập.

Nếu hủy kích hoạt của bạn bị trì hoãn, hãy làm theo các bước sau đây:

1. Nếu bạn đang hủy kích hoạt vai trò người quản trị Exchange hoặc thời hạn kích hoạt vai trò hết hạn, và bạn nhận thấy sự chậm trễ đáng kể trước khi các quyền được loại bỏ, hãy mở một vé hỗ trợ và thông báo cho kỹ sư hỗ trợ của bạn để giúp bạn gửi một vé với nhóm quản lý truy nhập đặc quyền (PAM) trong Office về vấn đề này.
2. Nếu thời gian kích hoạt đã hết hạn, nhưng bạn vẫn đang mở phiên trình duyệt, hãy đóng trình duyệt của bạn. Bạn có thể tiếp tục sử dụng vai trò cho đến khi bạn đóng phiên đó. Đây là một vấn đề đã biết và chúng tôi đang tìm kiếm một bản sửa lỗi nhằm kích hoạt lại mỗi phiên đã hết hạn.

Nếu sự chậm trễ của bạn khác với hai kịch bản này, vui lòng mở một vé hỗ trợ.
