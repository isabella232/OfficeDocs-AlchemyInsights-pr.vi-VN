---
title: Khắc phục lỗi 0x8004de40 trong OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755870"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Khắc phục lỗi 0x8004de40 trong OneDrive

Nếu bạn nhận được lỗi 0x8004de40 với OneDrive:

- Khởi động lại máy tính bị ảnh hưởng trong khi kết nối với miền Acitve thư mục của bạn.
- Nếu khởi động lại không khắc phục sự cố, hủy tham gia và kết nối lại thiết bị của bạn từ Azure AD. 

**Lưu ý**: bạn nên trên mạng công ty của bạn trong khi thực hiện các bước sau. Không thực hiện các bước này khi bạn không thể kết nối với cơ sở hạ tầng doanh nghiệp của mình (ví dụ: khi đang đi du lịch). 

- Mở dấu nhắc lệnh nâng cao. 
- Để mở dấu nhắc lệnh nâng cao, bấm- **bắt đầu**, bấm chuột phải vào **dấu nhắc lệnh**, và sau đó nhấp vào **chạy như quản trị viên**.
- Nhập *dsregcmd/để lại* và nhấn **Enter**.
- Khi hoàn tất, nhập *dsregcmd/tham gia* và nhấn **Enter**.
- Khi hoàn tất, đóng dấu nhắc lệnh.
- Khởi động lại máy tính và đăng nhập vào OneDrive.