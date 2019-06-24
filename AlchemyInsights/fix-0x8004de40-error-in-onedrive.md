---
title: Khắc phục lỗi 0x8004de40 trong OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133998"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Khắc phục lỗi 0x8004de40 trong OneDrive

Nếu bạn nhận được một lỗi 0x8004de40 với OneDrive:

- Khởi động lại máy tính bị ảnh hưởng, trong khi kết nối với miền Acitve thư mục của bạn.
- Nếu khởi động lại không giải quyết vấn đề, unjoin và quay trở lại điện thoại từ các quảng cáo Azure. 

**Lưu ý**: bạn nên trên mạng doanh nghiệp của bạn trong khi thực hiện các bước sau. Không thực hiện các bước sau khi bạn không thể kết nối với cơ sở hạ tầng công ty của bạn (ví dụ, trong khi đi du lịch). 

- Mở một dấu nhắc lệnh nâng lên. 
- Để mở một dấu nhắc lệnh cao, nhấp vào - **bắt đầu**, bấm chuột phải vào **dấu nhắc lệnh**và sau đó nhấp vào **chạy như quản trị**.
- Nhập *dsregcmd /leave* và nhấn **Enter**.
- Khi hoàn tất, nhập *dsregcmd /join* và nhấn **Enter**.
- Khi hoàn thành, đóng dấu nhắc lệnh.
- Khởi động lại máy tính và đăng nhập vào OneDrive.