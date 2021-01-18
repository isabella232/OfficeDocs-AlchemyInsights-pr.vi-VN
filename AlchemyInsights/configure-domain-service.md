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
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885784"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Không thể bật không kích hoạt được-DS hoặc triển khai

Để giải quyết vấn đề dịch vụ Azure AD Domain (không được bật hoặc không cho phép triển khai, hãy thực hiện các bước sau đây:

1. Nếu bạn đang sử dụng một mạng ảo hiện có, hãy kiểm tra NSG của bạn để quy tắc chặn các cổng cần thiết để đồng bộ hóa trong thiết bị in-DS trong cổng thông tin https://aka.ms/aadds-networking .
2. Kiểm tra xem thông báo lỗi của bạn được trả lời trong hướng dẫn khắc phục sự cố này sẵn dùng hay không  https://aka.ms/aadds-troubleshoot-enable .
3. Thử triển khai các dịch vụ tên miền Azure AD trong một mạng ảo mới.
4. Làm theo hướng dẫn bắt đầu về cách triển khai thiết [lập: tạo và đặt cấu hình dịch vụ miền](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)của bạn.
5. Nếu bạn đang gặp vấn đề khi triển khai Azure AD Domain Services, hãy xem [khắc phục sự cố dịch vụ AZURE AD Domain](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) để giải quyết các lỗi thường gặp để giúp bạn làm việc cùng một lần nữa. 

**Không thể tắt tính năng đọc tiếng Anh**

Không thể tạm dừng không đọc được. Nếu bạn muốn ngừng sử dụng tên miền được quản lý của mình, nó phải bị xóa bỏ.
Để xóa tên miền được quản lý của bạn, hãy xem [xóa dịch vụ tên miền AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



