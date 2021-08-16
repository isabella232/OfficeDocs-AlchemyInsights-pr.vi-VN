---
title: Nhiều người dùng bị lỗi Truy nhập Bị từ chối trong khi thêm phần bổ trợ trong Outlook
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
ms.openlocfilehash: 5e5f881ad72d2a0f76c8659d6b1044bf6a18464fa8d65c079e44eb1a2afd4431
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065414"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Nhiều người dùng bị lỗi Truy nhập Bị từ chối trong khi thêm phần bổ trợ trong Outlook

Bạn có thể chỉ định người quản trị trong tổ chức của mình có quyền cài đặt và quản lý các phần bổ trợ dành cho Outlook. Bạn cũng có thể chỉ định người dùng nào trong tổ chức của bạn có quyền cài đặt và quản lý các phần bổ trợ để sử dụng riêng.

Để biết chi tiết, hãy xem Chỉ định người quản trị và người dùng có thể cài [đặt và quản lý phần bổ trợ Outlook.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)

Để xác minh rằng bạn đã gán thành công các quyền cho người dùng, hãy thay bằng tên của vai trò đó để xác minh và chạy lệnh sau <Role Name> đây trong Exchange Online PowerShell:

Get-ManagementRoleAssignment -Role " <Role Name> " -GetEffectiveUsers

Ví dụ này cho bạn thấy cách xác minh xem bạn đã gán quyền để cài đặt các phần bổ trợ từ Office Store cho tổ chức.

Powershell

-Role "Org Marketplace Apps" -GeteffectiveUsers

Trong kết quả, Get-ManagementRoleAssignment, xem lại các mục nhập trong cột Người dùng Hiệu quả.

Để biết thông tin về cú pháp và tham số chi [tiết, hãy xem Get-ManagementRoleAssignment.](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)
 