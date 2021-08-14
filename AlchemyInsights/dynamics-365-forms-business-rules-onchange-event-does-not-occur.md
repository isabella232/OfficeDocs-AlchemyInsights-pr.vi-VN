---
title: Quy tắc Kinh doanh của Dynamics 365 Forms - Quy tắc Doanh nghiệp Không Được sử dụng cho Biểu mẫu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947321"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Sự kiện OnChange sẽ không xảy ra nếu trường bị thay đổi theo chương trình

Sự *kiện OnChange* sẽ không xảy ra nếu trường được thay đổi theo chương trình bằng cách sử dụng thuộc *tính.* [phương pháp setValue.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Nếu bạn muốn bộ xử lý sự kiện cho sự kiện *OnChange* chạy sau khi đã đặt giá trị thì bạn phải sử dụng phương pháp *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) trong mã của mình.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
