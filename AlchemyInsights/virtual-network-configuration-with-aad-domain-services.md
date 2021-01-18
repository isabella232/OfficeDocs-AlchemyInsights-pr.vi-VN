---
title: Cấu hình ảo với dịch vụ tên miền của Bad
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
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885781"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Cấu hình ảo với dịch vụ tên miền của Bad

Cấu hình ảo với dịch vụ tên miền của Bad liên quan đến các bước sau đây: 

1. Kiểm tra trạng thái tên miền của bạn trên cổng thông tin Azure https://aka.ms/aadds-health
2. Kiểm tra NSG của bạn để xem các quy tắc chặn cổng cần thiết để đồng bộ hóa trong dịch vụ tên miền Azure AD trên cổng thông tin https://aka.ms/aadds-networking
3. Đảm bảo rằng mạng ảo của bạn được triển khai trong cùng một vùng Azure với tên miền Azure AD Domain Services của bạn.
4. Đảm bảo bạn không có tên miền nào có cùng tên miền sẵn dùng trên mạng ảo.

Để biết thêm chi tiết về việc xem xét thiết kế trên Azure Virtual Network để hỗ trợ dịch vụ tên miền của Bad, hãy xem [xem xét mạng ảo](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

