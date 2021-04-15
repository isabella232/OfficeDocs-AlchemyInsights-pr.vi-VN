---
title: Khắc phục lỗi 0x8005de40 trong OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649770"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Khắc phục lỗi 0x8005de40 trong OneDrive

Nếu bạn đang chạy Windows 7 và nhận được thông báo lỗi này, hãy [Cập Nhật để bật tls 1,1 và tls 1,2 là các giao thức bảo mật mặc định trong WinHTTP trong Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

Nếu bạn đang chạy Windows 10 và bạn nhận được lỗi 0x8005de40 với OneDrive:

- Khởi động lại máy tính bị ảnh hưởng khi đã kết nối với tên miền Acitve Directory của bạn.
- Nếu khởi động lại không khắc phục sự cố, hãy bỏ tham gia và gia nhập lại thiết bị của bạn từ Azure AD. 

**Lưu ý**: bạn nên có trong mạng công ty của bạn trong khi thực hiện các bước này. Không thực hiện các bước này khi bạn không được kết nối với cơ sở hạ tầng công ty của bạn (ví dụ, trong khi đang đi du lịch). 

1. Mở dấu nhắc lệnh nâng cao bằng cách chọn **bắt đầu**, bấm chuột phải vào **dấu nhắc lệnh**, rồi chọn **chạy với tư cách là người quản trị**.

1. Nhập *dsregcmd/Leave* và nhấn **Enter**.

1. Khi hoàn thành, nhập *dsregcmd/join* và nhấn **Enter**.

1. Khi hoàn thành, hãy đóng dấu nhắc lệnh.

1. Khởi động lại máy tính và đăng nhập vào OneDrive.