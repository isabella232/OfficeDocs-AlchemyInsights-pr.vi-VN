---
title: Vị trí dữ liệu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627868"
---
# <a name="data-location"></a>Vị trí dữ liệu

Bạn có thể xem vị trí của người thuê văn phòng 365 trong Trung tâm quản trị hoặc bằng cách kết nối với Exchange Online qua PowerShell.


**Trung tâm quản trị:**
1. Đăng nhập vào [Trung tâm quản trị](https://admin.microsoft.com/Adminportal/Home).
2. Chọn**cấu hình tổ chức** **cài đặt** > .
3. Trong **vị trí dữ liệu**, chọn **xem chi tiết**.


**Powershell:**
1. Kết nối với Exchange Online bằng cách sử dụng Windows PowerShell.
2. Thực hiện lệnh [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) để hiển thị danh sách các thuộc tính của người thuê. 
3. Xem thuộc tính OrganizationId.

Khi bạn có vị trí dữ liệu cho EXO và SPO, bạn có thể xác định vị trí dữ liệu cho các dịch vụ khác mà bạn có thể sử dụng từ [nơi dữ liệu của bạn nằm ở đâu](https://products.office.com/where-is-your-data-located).