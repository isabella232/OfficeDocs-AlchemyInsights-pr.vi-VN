---
title: Cấu hình dịch vụ miền
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
- "7931"
- "9004400"
ms.openlocfilehash: cf8ea7d73adf36f71ae92abad48ef9b664eb0c96094a38750c86cf42958b5323
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994795"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Không thể bật AAD-DS hoặc triển khai không thành công

Để giải quyết sự cố dịch vụ miền Azure AD (AAD-DS) chưa được kích hoạt hoặc triển khai không thành công, hãy thực hiện các bước sau đây:

1. Nếu bạn đang sử dụng một mạng ảo đã có sẵn, hãy kiểm tra NSG của bạn để biết các quy tắc chặn các cổng cần để đồng bộ hóa trong AAD-DS trong cổng thông tin https://aka.ms/aadds-networking .
2. Kiểm tra xem thông báo lỗi của bạn có được trả lời trong hướng dẫn khắc phục sự cố này không. https://aka.ms/aadds-troubleshoot-enable
3. Hãy thử triển khai Azure AD Domain Services trong mạng ảo mới.
4. Làm theo hướng dẫn Bắt đầu về cách triển khai AAD-DS: [Tạo và Đặt cấu hình Dịch vụ Miền AAD.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)
5. Nếu bạn đang gặp sự cố với việc Triển khai Dịch vụ Miền Azure AD, hãy xem mục Khắc phục sự cố Dịch vụ Miền [Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) để giải quyết các lỗi thường gặp để giúp bạn làm lại mọi việc. 

**Không thể vô hiệu hóa AAD-DS**

AAD-DS không thể tạm dừng. Nếu bạn muốn ngừng sử dụng tên miền được quản lý của mình, nó phải bị xóa.
Để xóa miền Được quản lý của bạn, hãy [xem mục Xóa Dịch vụ Miền AAD.](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds)



