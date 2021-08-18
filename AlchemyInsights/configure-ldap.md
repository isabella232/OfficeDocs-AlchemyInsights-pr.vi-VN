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
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090434"
---
# <a name="configure-ldap"></a>Đặt cấu hình LDAP

Để đặt cấu hình LDAP, hãy làm như sau:

1. Kiểm tra tình trạng miền của bạn trên cổng [thông tin Azure.](https://aka.ms/aadds-health)
1. Đảm bảo có sẵn đăng ký Azure AD hợp lệ và Dịch vụ Miền Azure AD đã được bật.
1. Chứng chỉ cần thiết để bật LDAP bảo mật phải được lấy từ một cơ quan chứng nhận công cộng đáng tin cậy hoặc là một chứng chỉ tự ký.
1. Ensure the certificate follow the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Chứng chỉ Không hợp lệ**
1. Để gia hạn một chứng chỉ, hãy làm theo các bước để tạo một chứng chỉ mới và tải lại: [Cấu hình LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. Để giải quyết sự cố đã biết với cảnh báo LDAP bảo mật trong Dịch vụ Miền Azure Active directory, hãy xem Giải [quyết cảnh báo LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
