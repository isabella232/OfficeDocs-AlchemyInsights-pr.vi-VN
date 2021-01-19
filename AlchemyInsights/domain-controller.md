---
title: Bộ điều khiển tên miền
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
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901319"
---
# <a name="domain-controller"></a>Bộ điều khiển tên miền

**Không thể bật không kích hoạt được-DS hoặc triển khai**

Để giải quyết vấn đề dịch vụ Azure AD Domain (không được bật hoặc không cho phép triển khai, hãy thực hiện các bước sau đây:

1. Nếu bạn đang sử dụng một mạng ảo hiện có, hãy kiểm tra NSG của bạn để quy tắc chặn các cổng cần thiết để đồng bộ hóa trong thiết bị in-DS trong cổng thông tin https://aka.ms/aadds-networking .
2. Kiểm tra xem thông báo lỗi của bạn được trả lời trong hướng dẫn khắc phục sự cố này sẵn dùng hay không  https://aka.ms/aadds-troubleshoot-enable .
3. Thử triển khai các dịch vụ tên miền Azure AD trong một mạng ảo mới.
4. Hãy làm theo hướng dẫn bắt đầu về cách triển khai các phép tiếp tục, vốn sẵn dùng tại mục [hướng dẫn để tạo Dịch vụ AZURE AD Domain](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Nếu bạn đang gặp vấn đề khi triển khai Azure AD Domain Services, hãy xem [khắc phục sự cố dịch vụ AZURE AD Domain](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) để giải quyết các lỗi thường gặp để giúp bạn làm việc cùng một lần nữa. 

**Không thể tắt tính năng đọc tiếng Anh**

Không thể tạm dừng không đọc được. Nếu bạn muốn ngừng sử dụng tên miền được quản lý của mình, nó phải bị xóa bỏ.

Nếu bạn gặp phải sự cố, để giải quyết thông báo lỗi thông thường và đối với các bước khắc phục sự cố liên kết để giúp bạn có thể chạy lại, hãy xem [khắc phục sự cố dịch vụ miền Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
