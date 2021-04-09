---
title: Khôi phục nhóm Microsoft 365 đã xóa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645153"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Khôi phục nhóm Microsoft 365 đã xóa

Bạn có thể khôi phục một nhóm Microsoft 365 đã xóa hoặc các nhóm Microsoft trong vòng 30 ngày kể từ khi xóa.

1. Đi đến [Trung tâm quản trị Microsoft 365](https://aka.ms/RestoreDeletedGroup) để đăng nhập vào danh sách bạn là nhóm và nhóm đã xóa.

    **Lưu ý:** Đăng nhập bằng cách sử dụng tài khoản được gán cho người quản trị đối tượng thuê hoặc vai trò quản trị nhóm.

1. Chọn Nhóm Microsoft 365/nhóm đã xóa sẽ được khôi phục và bấm **khôi phục nhóm**.

    Nếu nhóm không thể khôi phục do địa chỉ SMTP xung đột, hãy dùng lệnh sau để tìm đối tượng gây ra xung đột và loại bỏ địa chỉ SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Lưu ý:** Trong một số trường hợp, có thể mất đến 24 giờ cho nhóm và tất cả dữ liệu của nó sẽ được khôi phục.

    Để biết thêm thông tin, hoặc để tìm hiểu cách khôi phục nhóm bằng PowerShell, hãy xem [khôi phục nhóm Microsoft 365 đã xóa](https://go.microsoft.com/fwlink/?linkid=867802).