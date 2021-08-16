---
title: Cấu hình ảo với dịch vụ tên miền AAD
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
- "7927"
- "9004397"
ms.openlocfilehash: 03a6ec63ba8e2779b0fe3f0381606af2c0748f8b848baaa7cd88b61317bd7a5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072866"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Cấu hình ảo với dịch vụ tên miền AAD

Cấu hình ảo với dịch vụ tên miền AAD bao gồm các bước sau đây: 

1. Kiểm tra tình trạng tên miền của bạn trên cổng thông tin Azure https://aka.ms/aadds-health
2. Kiểm tra NSG của bạn xem có quy tắc chặn các cổng cần thiết để đồng bộ hóa trong Azure AD Domain Services trên cổng thông tin https://aka.ms/aadds-networking
3. Đảm bảo rằng mạng ảo của bạn được triển khai trong cùng một Khu vực Azure với miền do Dịch vụ Miền Azure AD quản lý.
4. Đảm bảo bạn không có tên miền hiện có với cùng một tên miền sẵn có trên mạng ảo.

Để biết thêm chi tiết về việc cân nhắc thiết kế trên Mạng Ảo Azure để hỗ trợ các dịch vụ miền AAD, hãy xem mục [Cân nhắc về mạng ảo.](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)

