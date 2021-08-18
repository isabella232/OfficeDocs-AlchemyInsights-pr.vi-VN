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
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324012"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Khắc phục các sự cố phổ biến với định dạng bản ghi DKIM

Hầu hết các vấn đề thiết lập DKIM đều liên quan đến bản ghi DNS không chính xác.

Để khắc phục các sự cố về thiết lập DKIM, hãy xác minh rằng bản ghi CNAME DKIM **(không** phải bản ghi TXT) được định dạng chính xác. Để biết thêm thông tin, hãy [xem mục Những việc bạn cần làm để thiết lập DKIM theo](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)cách thủ Office 365.

Nếu bạn cần trợ giúp về bản ghi DNS nói chung, hãy xem Tạo bản [ghi DNS tại nhà cung cấp lưu trữ DNS bất kỳ Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

**Lưu** ý: Sau khi bạn tạo hoặc cập nhật bản ghi DNS DKIM của mình tại dịch vụ lưu trữ DNS cho miền của mình, bạn sẽ cần đợi các bản ghi DNS phát sinh.
