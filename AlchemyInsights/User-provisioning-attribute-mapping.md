---
title: Ánh xạ thuộc tính cung cấp người dùng
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 73da476cc5913a16911839a59b80959d3c99a8bc22471febe421b022ce2c49ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918165"
---
# <a name="user-provisioning-attribute-mapping"></a>Ánh xạ thuộc tính cung cấp người dùng

1. Để khắc phục sự cố ánh xạ thuộc tính đã biết, hãy xem [Ánh xạ thuộc tính](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Microsoft Azure Active Directory (AD) cung cấp hỗ trợ cho người dùng việc cung cấp cho các ứng dụng SaaS của bên thứ ba như Salesforce, G Suite và những ứng dụng khác. Nếu bạn cho phép người dùng cung cấp cho ứng dụng SaaS của bên thứ ba, cổng thông tin Azure sẽ điều khiển các giá trị thuộc tính thông qua ánh xạ thuộc tính. Để tìm hiểu cách tùy chỉnh ánh xạ thuộc tính mặc định, hãy xem mục Tùy chỉnh người dùng cung cấp thuộc tính-ánh xạ cho các ứng dụng [SaaS trong Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes)
    - Để tìm hiểu thêm về việc cung cấp người dùng ứng dụng SaaS, hãy xem mục Người dùng ứng dụng [SaaS](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) tự động cung cấp những gì trong Azure AD? 
3. Khi tùy chỉnh ánh xạ thuộc tính để cung cấp cho người dùng, bạn có thể thấy rằng thuộc tính bạn muốn ánh xạ không xuất hiện trong danh sách thuộc tính Nguồn. Đồng bộ một thuộc tính từ Active Directory tại chỗ của bạn với [Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) để cung cấp vào một bài viết ứng dụng cho bạn biết cách thêm thuộc tính bị thiếu bằng cách đồng bộ thuộc tính đó từ AD tại chỗ của bạn với Azure AD.
