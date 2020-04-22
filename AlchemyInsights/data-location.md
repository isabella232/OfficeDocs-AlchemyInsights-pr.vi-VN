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
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655304"
---
# <a name="data-location"></a>Vị trí dữ liệu

Bạn có thể xem vị trí của đối tượng thuê của bạn trong Trung tâm quản trị hoặc bằng cách kết nối với Exchange Online qua PowerShell.


**Trung tâm quản trị:**
1. Đăng nhập vào [Trung tâm quản trị](https://admin.microsoft.com/Adminportal/Home).
2. Chọn**cấu hình tổ chức** **cài đặt** > .
3. Trong **vị trí dữ liệu**, chọn **xem chi tiết**.


**Powershell:**
1. Kết nối với Exchange Online bằng cách sử dụng Windows PowerShell.
2. Thực hiện lệnh [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) để hiển thị danh sách các thuộc tính của người thuê. 
3. Xem thuộc tính OrganizationId.

Khi bạn có vị trí dữ liệu cho EXO và SPO, bạn có thể xác định vị trí dữ liệu cho các dịch vụ khác mà bạn có thể sử dụng từ [nơi dữ liệu của bạn nằm ở đâu](https://products.office.com/where-is-your-data-located).