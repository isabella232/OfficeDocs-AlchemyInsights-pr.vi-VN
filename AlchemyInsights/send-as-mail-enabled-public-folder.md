---
title: Gửi Dưới dạng Thư mục Công cộng hỗ trợ Thư trong EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 22aa3e8f46c2ff4f62cb520b9498041dffb9d3a3eb607d788cc97b10bf32dbb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052588"
---
# <a name="sendas-mail-enabled-public-folder"></a>Thư mục Công cộng hỗ trợ Thư SendAs

Ví dụ sau gán quyền "Gửi Với tư cách" cho thư mục công cộng hỗ trợ thư NewPF1 cho người dùng Jason.

Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'

Để biết thông tin về cú pháp và tham số chi tiết, hãy xem mục Gán quyền "Gửi Với tư cách" hoặc "Gửi Thay mặt" cho thư [mục công cộng hỗ trợ thư.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)

