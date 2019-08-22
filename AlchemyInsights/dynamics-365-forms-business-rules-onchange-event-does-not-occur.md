---
title: Dynamics 365 tạo quy tắc kinh doanh - nguyên tắc kinh doanh không bắn cho một hình thức
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529041"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Sự kiện Ajax không xảy ra nếu lĩnh vực là thay đổi lập trình

Sự kiện *Ajax* không xảy ra nếu lĩnh vực này đã thay đổi lập trình bằng cách sử dụng các *tính.* phương thức [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Nếu bạn muốn xử lý sự kiện cho các sự kiện *Ajax* chạy sau khi bạn thiết lập giá trị bạn phải sử dụng các *thuộc tính formContext.data.entity.* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) các phương pháp trong mã của bạn.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
