---
title: Dynamics 365 Forms quy định kinh doanh-quy tắc kinh doanh không bắn cho một mẫu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769361"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Sự kiện Ajax xảy ra nếu trường được thay đổi lập

Sự kiện *Ajax* xảy ra nếu trường được thay đổi lập bằng cách sử dụng các *thuộc tính.* phương pháp [Setvalue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Nếu bạn muốn xử lý sự kiện *onChange* sự kiện chạy sau khi bạn đặt giá trị bạn phải sử dụng các *thuộc tính formcontext. Data. ENTITY* phương pháp [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) trong mã của bạn.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
