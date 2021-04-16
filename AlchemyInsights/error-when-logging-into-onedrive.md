---
title: lỗi 0x8006de40 khi khởi chạy OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813674"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>lỗi 0x8006de40 khi khởi chạy OneDrive

Nếu bạn nhận được lỗi **0x8005de40** khi đăng nhập vào OneDrive, hãy khởi động lại máy tính khi kết nối với tên miền cơ quan hoặc trường học của bạn. Nếu bạn nhận được lỗi này sau khi khởi động lại, hãy thử điều này khi được kết nối với tên miền cơ quan hoặc trường học của bạn:

1. Bấm vào bắt đầu, rồi nhập **CMD** hoặc **Command Prompt**  vào hộp tìm kiếm, bấm chuột phải vào ứng dụng nhắc lệnh, rồi chọn  **chạy với tư trình quản trị**. Nếu bạn được nhắc nhập mật khẩu người quản trị hoặc để xác nhận, hãy nhập mật khẩu hoặc bấm **cho phép**.  

2. Trong cửa sổ dấu nhắc lệnh, nhập **dsregcmd/Leave**  và wait cho lệnh để hoàn thành. Sau đó, nhập **dsregcmd/join** và chờ lệnh để hoàn thành.
3. Khởi động lại máy tính của bạn.
