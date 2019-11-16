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
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="fdc29-102">Sự kiện Ajax xảy ra nếu trường được thay đổi lập</span><span class="sxs-lookup"><span data-stu-id="fdc29-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="fdc29-103">Sự kiện *Ajax* xảy ra nếu trường được thay đổi lập bằng cách sử dụng các *thuộc tính.* phương pháp [Setvalue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) .</span><span class="sxs-lookup"><span data-stu-id="fdc29-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="fdc29-104">Nếu bạn muốn xử lý sự kiện *onChange* sự kiện chạy sau khi bạn đặt giá trị bạn phải sử dụng các *thuộc tính formcontext. Data. ENTITY* phương pháp [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) trong mã của bạn.</span><span class="sxs-lookup"><span data-stu-id="fdc29-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
