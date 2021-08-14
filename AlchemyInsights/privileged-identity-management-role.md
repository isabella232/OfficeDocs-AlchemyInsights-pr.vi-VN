---
title: Privileged Identity Management vai trò
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
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973251"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management vai trò (PIM)

**Các quyền không được cấp sau khi kích hoạt vai trò**

Khi bạn kích hoạt vai trò trong Azure AD Privileged Identity Management (PIM), kích hoạt có thể không ngay lập tức phát sinh đến tất cả các cổng thông tin yêu cầu vai trò có đặc quyền. Đôi khi, ngay cả khi thay đổi này được phát tán, thì việc lưu bộ nhớ đệm web trong cổng thông tin có thể dẫn đến việc thay đổi không có hiệu lực ngay lập tức.

Nếu kích hoạt của bạn bị trì hoãn, hãy làm theo các bước sau:

1. Đăng xuất khỏi cổng thông tin Azure, rồi đăng nhập lại. Khi bạn kích hoạt vai trò Azure AD hoặc vai trò tài nguyên Azure, bạn sẽ thấy các giai đoạn kích hoạt. Sau khi tất cả các giai đoạn đã hoàn tất, bạn sẽ thấy liên kết 'Đăng xuất'. Bạn có thể sử dụng liên kết này để đăng xuất. Điều này sẽ giải quyết hầu hết các trường hợp về độ trễ kích hoạt.
2. Trong mã PIM, hãy xác nhận rằng bạn được liệt kê là thành viên của vai trò đó.
3. Nếu bạn đang kích hoạt vai Exchange Người quản trị, hãy đảm bảo bạn đăng xuất, rồi đăng nhập lại. Nếu sự cố vẫn tiếp diễn, hãy mở một thẻ hỗ trợ và nêu vấn đề này. Nếu bạn đang sử dụng vai trò Người quản Exchange quản trị để truy nhập Trung tâm Bảo mật và Tuân thủ, hãy xem bước tiếp theo.
4. Nếu bạn đang kích hoạt vai trò để truy nhập vào Trung tâm Bảo mật và Tuân thủ hoặc nếu bạn đang kích hoạt vai trò Người quản trị SharePoint, bạn sẽ gặp phải một số trì hoãn kích hoạt từ vài phút đến vài giờ. Đây là vấn đề đã biết và chúng tôi đang tích cực làm việc với các nhóm này để giải quyết vấn đề này càng sớm càng tốt.

Để biết thêm thông tin, hãy xem:

- [Kích hoạt vai trò Azure AD của tôi trong pim](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Kích hoạt vai trò tài nguyên Azure của tôi trong PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Các quyền sẽ không bị loại bỏ sau khi hủy kích hoạt vai trò hoặc kích hoạt vai trò sẽ hết hạn**

Khi bạn hủy kích hoạt vai trò trong Azure AD Privileged Identity Management hoặc khi thời gian kích hoạt vai trò hết hạn, bạn có thể phải chờ để tiếp tục có quyền truy nhập.

Nếu việc hủy kích hoạt của bạn bị trì hoãn, hãy làm theo các bước sau:

1. Nếu bạn hủy kích hoạt vai trò Người quản trị Exchange hoặc thời gian kích hoạt vai trò sẽ hết hạn và bạn nhận thấy sự chậm trễ đáng kể trước khi các quyền bị loại bỏ, hãy mở phiếu hỗ trợ và yêu cầu kỹ sư hỗ trợ giúp bạn gửi phiếu vào nhóm Quản lý Truy nhập Đặc quyền (PAM) bên trong Office về sự cố này.
2. Nếu thời gian kích hoạt đã hết hạn nhưng bạn vẫn mở phiên trình duyệt, hãy đóng trình duyệt của bạn. Bạn có thể tiếp tục sử dụng vai trò này cho đến khi bạn đóng phiên đó. Đây là sự cố đã biết và chúng tôi đang tìm kiếm bản sửa lỗi tiềm năng để chủ động thu hồi từng phiên sau khi kích hoạt đã hết hạn.

Nếu độ trễ của bạn khác với hai kịch bản này, vui lòng mở một vé hỗ trợ.
