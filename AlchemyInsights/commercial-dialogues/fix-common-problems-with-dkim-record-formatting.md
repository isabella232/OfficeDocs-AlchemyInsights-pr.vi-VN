---
title: Khắc phục các sự cố phổ biến với định dạng bản ghi DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930083"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Khắc phục các sự cố phổ biến với định dạng bản ghi DKIM

Hầu hết các vấn đề thiết lập DKIM đều liên quan đến bản ghi DNS không chính xác.

Để khắc phục các sự cố về thiết lập DKIM, hãy xác minh rằng bản ghi CNAME DKIM **(không** phải bản ghi TXT) được định dạng chính xác. Để biết thêm thông tin, [hãy xem mục Những việc bạn cần làm để thiết lập DKIM theo cách thủ Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Nếu bạn cần trợ giúp về bản ghi DNS nói chung, hãy xem Tạo bản ghi DNS tại nhà cung cấp [lưu trữ DNS bất kỳ Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> Sau khi tạo hoặc cập nhật bản ghi DNS DKIM của mình tại dịch vụ lưu trữ DNS cho miền của mình, bạn sẽ cần chờ các bản ghi DNS phát sinh.
