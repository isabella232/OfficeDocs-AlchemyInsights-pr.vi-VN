---
title: Khắc phục lỗi 0x8004de40 trong OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716050"
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