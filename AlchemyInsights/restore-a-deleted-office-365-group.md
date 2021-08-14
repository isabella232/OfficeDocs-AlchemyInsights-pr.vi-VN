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
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959048"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Khôi phục nhóm Microsoft 365 đã xóa

Bạn có thể khôi phục nhóm Microsoft 365 đã xóa hoặc Microsoft Teams trong vòng 30 ngày kể từ khi xóa.

1. Đi tới trang [Trung tâm quản trị Microsoft 365](https://aka.ms/RestoreDeletedGroup) đăng nhập vào danh sách các nhóm và nhóm đã xóa của bạn.

    **Lưu ý:** Đăng nhập bằng tài khoản được gán cho người quản trị đối tượng thuê hoặc vai trò người quản trị nhóm.

1. Chọn nhóm/Microsoft 365 xóa bỏ để Teams khôi phục và bấm **khôi phục nhóm.**

    Nếu không thể khôi phục nhóm do địa chỉ SMTP xung đột, hãy sử dụng lệnh sau đây để tìm đối tượng đang gây xung đột và loại bỏ địa chỉ SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Lưu ý:** Trong một số trường hợp, có thể mất đến 24 giờ để khôi phục nhóm và toàn bộ dữ liệu của nhóm.

    Để biết thêm thông tin hoặc để tìm hiểu cách khôi phục nhóm bằng PowerShell, hãy xem [khôi phục nhóm Microsoft 365 xóa](https://go.microsoft.com/fwlink/?linkid=867802).