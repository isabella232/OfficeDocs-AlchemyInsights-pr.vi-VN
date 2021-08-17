---
title: Bộ điều khiển miền
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: b044e69cef177c5a1ad38c2d27a297d90ba7f55e7b2e75fff2e390869241f325
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057916"
---
# <a name="domain-controller"></a>Bộ điều khiển miền

**Không thể bật AAD-DS hoặc triển khai không thành công**

Để giải quyết sự cố dịch vụ miền Azure AD (AAD-DS) chưa được kích hoạt hoặc triển khai không thành công, hãy thực hiện các bước sau đây:

1. Nếu bạn đang sử dụng một mạng ảo đã có sẵn, hãy kiểm tra NSG của bạn để biết các quy tắc chặn các cổng cần để đồng bộ hóa trong AAD-DS trong cổng thông tin https://aka.ms/aadds-networking .
2. Kiểm tra xem thông báo lỗi của bạn có được trả lời trong hướng dẫn khắc phục sự cố này không. https://aka.ms/aadds-troubleshoot-enable
3. Hãy thử triển khai Azure AD Domain Services trong mạng ảo mới.
4. Làm theo hướng dẫn Bắt đầu về cách triển khai AAD-DS, có trong Hướng dẫn [để Tạo Dịch vụ Miền Azure AD.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)
5. Nếu bạn đang gặp sự cố với việc Triển khai Dịch vụ Miền Azure AD, hãy xem mục Khắc phục sự cố Dịch vụ Miền [Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) để giải quyết các lỗi thường gặp để giúp bạn làm lại mọi việc. 

**Không thể vô hiệu hóa AAD-DS**

AAD-DS không thể tạm dừng. Nếu bạn muốn ngừng sử dụng tên miền được quản lý của mình, nó phải bị xóa.

Nếu bạn gặp phải sự cố, để giải quyết các thông báo lỗi thường gặp và để biết các bước khắc phục sự cố liên quan giúp bạn bắt đầu lại, hãy xem Khắc [phục Azure Active Directory Dịch](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)vụ Miền .
