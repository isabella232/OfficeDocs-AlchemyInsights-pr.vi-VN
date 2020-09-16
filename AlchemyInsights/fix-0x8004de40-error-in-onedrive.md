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
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745152"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Khắc phục lỗi 0x8005de40 trong OneDrive

Nếu bạn nhận được lỗi 0x8005de40 với OneDrive:

- Khởi động lại máy tính bị ảnh hưởng khi đã kết nối với tên miền Acitve Directory của bạn.
- Nếu khởi động lại không khắc phục sự cố, hãy bỏ tham gia và gia nhập lại thiết bị của bạn từ Azure AD. 

**Lưu ý**: bạn nên có trong mạng công ty của bạn trong khi thực hiện các bước này. Không thực hiện các bước này khi bạn không thể kết nối với cơ sở hạ tầng công ty của bạn (ví dụ, trong khi đang đi du lịch). 

- Mở một dấu nhắc lệnh nâng cao. 
- Để mở dấu nhắc lệnh nâng cao, hãy bấm vào **bắt đầu**, bấm chuột phải vào **dấu nhắc lệnh**, rồi bấm vào **chạy với tư cách là người quản trị**.
- Nhập *dsregcmd/Leave* và nhấn **Enter**.
- Khi hoàn thành, nhập *dsregcmd/join* và nhấn **Enter**.
- Khi hoàn thành, hãy đóng dấu nhắc lệnh.
- Khởi động lại máy tính và đăng nhập vào OneDrive.