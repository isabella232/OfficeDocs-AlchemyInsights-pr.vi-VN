---
title: Sự cố với nhóm bảo mật
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: d8a3c011a3a7cba6c0b1cd00ac0eb587b75bbb5b06d96ef9fd75313734e74fd0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925763"
---
# <a name="issue-with-security-groups"></a>Sự cố với nhóm bảo mật

**Nếu bạn gặp Lỗi Mạng AADDS104**

Quy tắc nhóm bảo mật mạng không hợp lệ là nguyên nhân phổ biến nhất gây ra lỗi mạng Azure Active Directory Dịch vụ Miền (AD DS). Nhóm bảo mật mạng cho mạng ảo phải cho phép truy nhập vào các cổng và giao thức cụ thể. Nếu các cổng này bị chặn, nền tảng Azure không thể theo dõi hoặc cập nhật miền được quản lý. Quá trình đồng bộ hóa giữa Azure AD và Azure AD DS cũng bị ảnh hưởng. Đảm bảo bạn luôn mở các cổng mặc định để tránh bị gián đoạn trong dịch vụ.

Để tìm hiểu và giải quyết các cảnh báo phổ biến về sự cố cấu hình nhóm bảo mật mạng, hãy xem [thêm và Xác minh Nhóm Bảo mật.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)
