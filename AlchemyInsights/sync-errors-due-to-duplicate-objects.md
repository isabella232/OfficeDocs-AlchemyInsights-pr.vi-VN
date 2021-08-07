---
title: 902 (Lỗi đồng bộ do các đối tượng trùng lặp)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998822"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Lỗi đồng bộ do các đối tượng trùng lặp

Bạn có thể nhận được một trong những thông báo lỗi sau đây khi quá trình đồng bộ hóa thư mục kết Microsoft 365:

- Không thể cập nhật đối tượng này trong Microsoft Online Services vì các thuộc tính sau được liên kết với đối tượng này có giá trị có thể đã được liên kết với một đối tượng khác trong thư mục cục bộ của bạn.

- Đối tượng được đồng bộ hóa với cùng địa chỉ proxy đã tồn tại trong thư mục Microsoft Online Services của bạn.

- Không thể cập nhật đối tượng này vì các thuộc tính sau được liên kết với đối tượng này có giá trị có thể đã được liên kết với một đối tượng khác trong dịch vụ thư mục cục bộ của bạn: UserPrincipalName.

Để xác định và khắc phục sự cố, hãy tải xuống và chạy Công cụ Khắc phục Lỗi [IdFix DirSync.](https://github.com/Microsoft/idfix)

Để biết thêm thông tin, [hãy xem KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
