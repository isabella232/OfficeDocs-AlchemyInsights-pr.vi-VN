---
title: Nhiều người dùng có thể truy cập từ chối lỗi khi thêm trình bổ sung trong Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424282"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Nhiều người dùng có thể truy cập từ chối lỗi khi thêm trình bổ sung trong Outlook

Bạn có thể chỉ định quản trị viên trong tổ chức của bạn có quyền để cài đặt và quản lý trình bổ sung cho Outlook. Bạn cũng có thể chỉ định người dùng nào trong tổ chức của bạn có quyền cài đặt và quản lý trình bổ sung để sử dụng riêng.

Để biết chi tiết, hãy xem [chỉ định quản trị viên và người dùng có thể cài đặt và quản lý trình bổ sung cho Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Để xác minh rằng bạn đã gán thành công các quyền cho người dùng, hãy thay thế <Role Name> bằng tên của vai trò đó để xác minh và chạy lệnh sau trong Exchange Online PowerShell:

Get-Managementrolegán-vai trò " <Role Name> "-geteffectiveusers

Ví dụ này cho bạn biết cách xác minh người mà bạn đã gán quyền để cài đặt trình bổ sung từ Office Store cho tổ chức.

Powershell

-Vai trò "ứng dụng org Marketplace"-GetEffectiveUsers

Trong kết quả, Get-Managementrolegán, đánh giá các mục trong cột hiệu quả người dùng.

Để biết cú pháp chi tiết và thông tin tham số, xem [Get-Managementrolegán](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 