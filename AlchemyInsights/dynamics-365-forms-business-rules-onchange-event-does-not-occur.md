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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/25/2019
ms.locfileid: "36529041"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Sự kiện Ajax xảy ra nếu trường được thay đổi lập

Sự kiện *Ajax* xảy ra nếu trường được thay đổi lập bằng cách sử dụng các *thuộc tính.* phương pháp [Setvalue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Nếu bạn muốn xử lý sự kiện *onChange* để chạy sau khi bạn đặt giá trị bạn phải sử dụng *thuộc tính formcontext. Data. ENTITY.* phương pháp [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) trong mã của bạn.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
