---
title: Động lực 365 biểu mẫu quy tắc kinh doanh-quy tắc kinh doanh không được bắn cho biểu mẫu
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
ms.openlocfilehash: 7422b67973f93ce10c1639209cc50206a1016c10
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711513"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Sự kiện OnChange không xảy ra nếu trường được thay đổi theo lập trình

Sự kiện *onChange* không xảy ra nếu trường được thay đổi theo chương trình bằng *thuộc tính.* phương pháp [Setvalue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Nếu bạn muốn xử lý sự kiện cho sự kiện *onChange* để chạy sau khi bạn thiết lập giá trị mà bạn phải dùng phương pháp điều chỉnh theo *ngữ cảnh. dữ liệu. thuộc tính* [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) thuộc tính trong mã của bạn.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
