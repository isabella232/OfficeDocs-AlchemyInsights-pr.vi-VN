---
title: Vấn đề với nhóm bảo mật
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
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177638"
---
# <a name="issue-with-security-groups"></a>Vấn đề với nhóm bảo mật

**Nếu bạn đang nhận được thông báo lỗi mạng AADDS104**

Các quy tắc nhóm bảo mật mạng không hợp lệ là nguyên nhân phổ biến nhất của các lỗi mạng cho Azure dịch vụ miền Active Directory (AD DS). Nhóm bảo mật mạng cho mạng ảo phải cho phép truy nhập vào các cổng và giao thức cụ thể. Nếu các cổng này bị chặn, nền tảng Azure không thể theo dõi hoặc Cập Nhật tên miền được quản lý. Đồng bộ hóa giữa các Azure AD và Azure AD DS cũng bị ảnh hưởng. Đảm bảo bạn tiếp tục mở cổng thông tin mặc định để tránh bị gián đoạn dịch vụ.

Để hiểu và giải quyết các vấn đề về cấu hình nhóm bảo mật mạng, hãy xem mục [Thêm và xác nhận nhóm bảo mật](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
