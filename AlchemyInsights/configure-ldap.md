---
title: Đặt cấu hình LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885775"
---
# <a name="configure-ldap"></a>Đặt cấu hình LDAP

Để đặt cấu hình LDAP, hãy làm như sau:

1. Kiểm tra trạng thái của tên miền của bạn trên [cổng thông tin Azure](https://aka.ms/aadds-health).
1. Đảm bảo đăng ký Azure AD hợp lệ có sẵn và dịch vụ tên miền Azure AD đã được bật.
1. Chứng chỉ được yêu cầu để bật LDAP bảo mật phải được lấy từ cơ quan chứng nhận công cộng đáng tin cậy hoặc chứng chỉ tự ký.
1. Đảm bảo chứng chỉ theo các [hướng dẫn](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)bắt buộc.

**Chứng chỉ không hợp lệ**
1. Để gia hạn chứng chỉ, hãy làm theo các bước để tạo chứng chỉ mới và tải lên lại: [đặt cấu hình LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Để giải quyết sự cố đã biết với cảnh báo an toàn của LDAP trong Azure Active Directory Services, hãy xem [giải quyết cảnh báo LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
