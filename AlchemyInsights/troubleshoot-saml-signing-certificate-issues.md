---
title: Khắc phục sự cố chứng chỉ ký vào SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694455"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Khắc phục sự cố chứng chỉ ký vào SAML

Để giải quyết sự cố về chứng chỉ ký hợp nhất, hãy thực hiện các bước được đề xuất sau đây:

1. Khi bạn thêm ứng dụng doanh nghiệp hỗ trợ SSO, Azure sẽ tạo ra một chứng chỉ được gọi là [chứng chỉ ký SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications). Chứng chỉ này có ngày hết hạn 3 năm. Để thay đổi ngày hết hạn chứng chỉ của bạn, hãy xem [tùy chỉnh ngày hết hạn cho chứng chỉ liên kết của bạn và cuộn nó sang chứng chỉ mới](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. Azure sẽ dùng chứng chỉ này để ký thẻ SAML được yêu cầu bởi ứng dụng và gửi qua ứng dụng cho một SSO thành công. Để hoàn tất việc này, hãy tải xuống chứng chỉ từ cổng thông tin Azure và gửi nó đến nhà cung cấp ứng dụng để hoàn tất quy trình SSO.

Sau khi quá trình này hoàn thành ứng dụng của bạn sẽ tin cậy chứng chỉ này và tất cả các thẻ SAML được ký bằng chứng chỉ này sẽ được ứng dụng chấp nhận.

3. Nếu chứng chỉ này hết hạn, hãy tạo chứng chỉ mới, Cập Nhật tài liệu đó vào nhà cung cấp ứng dụng, rồi làm cho nó hiện hoạt trên Azure bên. Để biết thêm thông tin, hãy xem gia [hạn một chứng chỉ sẽ sớm hết hạn](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

> [!NOTE]
> Nếu chứng chỉ hết hạn, thì người dùng sẽ không bị chặn.

4. [Thêm một địa chỉ email để nhận thông báo](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) sẽ được nhận trước khi chứng chỉ hiện tại hết hạn.

> [!NOTE]
> Bước-4 là một tùy chọn.

5. Thay đổi tùy chọn ký chứng chỉ SAML của ứng dụng và thuật toán ký chứng chỉ. Để biết thêm thông tin, hãy xem mục [thay đổi tùy chọn ký chứng chỉ và thuật toán ký](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

