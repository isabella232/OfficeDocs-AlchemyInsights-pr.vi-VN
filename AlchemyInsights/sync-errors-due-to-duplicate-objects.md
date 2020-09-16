---
title: 902 (lỗi đồng bộ do các đối tượng trùng lặp)
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
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737363"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Lỗi đồng bộ do các đối tượng trùng lặp

Bạn có thể nhận được một trong các thông báo lỗi sau đây khi đồng bộ hóa thư mục kết thúc trong Microsoft 365:

- Không thể cập nhật đối tượng này trong Microsoft Online Services vì các thuộc tính sau được liên kết với đối tượng này có các giá trị mà có thể đã được liên kết với một đối tượng khác trong thư mục cục bộ của bạn.

- Một đối tượng đã đồng bộ với cùng địa chỉ proxy đã tồn tại trong danh bạ Microsoft Online Services của bạn.

- Không thể cập nhật đối tượng này vì các thuộc tính sau được liên kết với đối tượng này có các giá trị mà có thể đã được liên kết với một đối tượng khác trong các dịch vụ thư mục cục bộ của bạn: UserPrincipalName.

Để xác định và khắc phục sự cố, hãy tải xuống và chạy [công cụ khắc phục lỗi không đồng bộ Idfix Dirsync](https://www.microsoft.com/download/details.aspx?id=36832).

Để biết thêm thông tin, hãy xem [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
