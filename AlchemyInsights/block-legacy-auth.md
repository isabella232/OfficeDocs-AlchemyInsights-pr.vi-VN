---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820200"
---
# <a name="blocking-legacy-authentication"></a>Chặn xác thực kế thừa

Kế thừa xác thực là một thuật ngữ tham chiếu đến một yêu cầu xác thực được thực hiện bởi:

- Máy khách Office cũ hơn không sử dụng xác thực hiện đại (ví dụ, ứng dụng khách Office 2010).

- Bất kỳ máy khách nào sử dụng các giao thức thư kế thừa chẳng hạn như IMAP/SMTP/POP3.

Để biết thêm thông tin về cách chặn xác thực thừa kế và bật xác thực hiện đại, hãy tham khảo việc [chặn xác thực kế thừa](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).

Mặc định bảo mật trong Azure Active Directory (Azure AD) giúp bảo vệ tổ chức của bạn dễ dàng hơn. Mặc định bảo mật chứa thiết đặt bảo mật được cấu hình sẵn cho các cuộc tấn công phổ biến.
Để biết thêm thông tin về mặc định về bảo mật, hãy tham khảo mục [mặc định về bảo mật là gì?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults). 

**Lưu ý**: nếu đối tượng thuê của bạn đã được tạo vào hoặc sau ngày 22 tháng 10, 2019, có thể bạn đang gặp phải hành vi mặc định bảo mật mới và đã có tính năng mặc định bảo mật được kích hoạt trong đối tượng thuê của bạn.  Trong một nỗ lực để bảo vệ tất cả người dùng của chúng tôi, mặc định bảo mật đang được triển khai cho tất cả các đối tượng thuê mới được tạo ra.
