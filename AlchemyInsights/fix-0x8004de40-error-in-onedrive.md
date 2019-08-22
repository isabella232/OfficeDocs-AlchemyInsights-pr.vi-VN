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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525081"
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