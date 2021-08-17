---
title: Khắc phục sự cố chứng chỉ ký SAML
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
ms.openlocfilehash: 290e740ccd7f3beac5b77e63c32c5b18c295070e6002dcdde44ce4a93f4330f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105698"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Khắc phục sự cố chứng chỉ KÝ SAML

Để giải quyết sự cố chứng chỉ KÝ SAML, hãy thực hiện các bước được đề xuất sau đây:

1. Khi bạn thêm một ứng dụng doanh nghiệp hỗ trợ SSO, Azure sẽ tạo ra một chứng chỉ được gọi là [chứng chỉ KÝ SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications) Chứng chỉ này có ngày hết hạn là 3 năm. Để thay đổi ngày hết hạn chứng chỉ của bạn, hãy xem mục Tùy chỉnh ngày hết hạn cho chứng chỉ liên kết của bạn và chuyển sang [chứng chỉ mới](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. Azure sẽ sử dụng chứng chỉ này để ký mã thông báo SAML do ứng dụng yêu cầu và gửi mã thông báo đó tới ứng dụng để nhận được SSO thành công. Để hoàn tất việc này, hãy tải xuống chứng chỉ từ cổng thông tin Azure và gửi nó đến nhà cung cấp ứng dụng để hoàn thành quy trình SSO.

After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.

3. Nếu chứng chỉ này hết hạn, hãy tạo một chứng chỉ mới, cập nhật chứng chỉ đó cho nhà cung cấp ứng dụng và sau đó làm cho chứng chỉ hiện hoạt ở phía Azure. Để biết thêm thông tin, [hãy xem mục Gia hạn chứng chỉ sẽ sớm hết hạn.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)

> [!NOTE]
> Nếu chứng chỉ hết hạn, người dùng sẽ không bị chặn.

4. [Thêm địa chỉ email để nhận thông](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) báo trước khi chứng chỉ hiện tại hết hạn.

> [!NOTE]
> Bước 4 là một bước tùy chọn.

5. Thay đổi tùy chọn ký chứng chỉ SAML của ứng dụng và giải thuật ký chứng chỉ. Để biết thêm thông tin, hãy xem mục [Thay đổi tùy chọn ký chứng chỉ và thuật toán ký.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)

