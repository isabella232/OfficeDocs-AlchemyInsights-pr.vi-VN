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
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35749183"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="2f3f5-102">Sự kiện Ajax không xảy ra nếu lĩnh vực là thay đổi lập trình</span><span class="sxs-lookup"><span data-stu-id="2f3f5-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="2f3f5-103">Sự kiện *Ajax* không xảy ra nếu lĩnh vực này đã thay đổi lập trình bằng cách sử dụng các *tính.* phương thức [setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) .</span><span class="sxs-lookup"><span data-stu-id="2f3f5-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="2f3f5-104">Nếu bạn muốn xử lý sự kiện cho các sự kiện *Ajax* chạy sau khi bạn thiết lập giá trị bạn phải sử dụng các *thuộc tính formContext.data.entity.* [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) các phương pháp trong mã của bạn.</span><span class="sxs-lookup"><span data-stu-id="2f3f5-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
