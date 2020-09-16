---
title: Nhiều người dùng bị từ chối truy nhập lỗi trong khi thêm phần bổ trợ trong Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724385"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Nhiều người dùng bị từ chối truy nhập lỗi trong khi thêm phần bổ trợ trong Outlook

Bạn có thể chỉ định người quản trị nào trong tổ chức của bạn có quyền cài đặt và quản lý các phần bổ trợ cho Outlook. Bạn cũng có thể xác định người dùng nào trong tổ chức của bạn có quyền cài đặt và quản lý các phần bổ trợ cho việc sử dụng riêng của họ.

Để biết chi tiết, hãy xem [mục xác định người quản trị và người dùng có thể cài đặt và quản lý các phần bổ trợ cho Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Để xác nhận rằng bạn đã gán quyền thành công cho một người dùng, hãy thay thế <Role Name> bằng tên của vai trò đó để xác nhận và chạy lệnh sau đây trong Exchange Online PowerShell:

Get-Managementrolegán vai trò " <Role Name> "-geteffectiveusers

Ví dụ này cho bạn biết cách xác minh người mà bạn đã gán quyền cài đặt phần bổ trợ từ Office Store cho tổ chức.

PowerShell

-Vai trò "tổ chức ứng dụng của thị trường"-GetEffectiveUsers

Trong các kết quả, Get-Managementrolegán, xem lại các mục nhập trong cột người dùng hiệu quả.

Để biết thông tin về cú pháp và tham số chi tiết, hãy xem [Get-Managementrolegán](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 