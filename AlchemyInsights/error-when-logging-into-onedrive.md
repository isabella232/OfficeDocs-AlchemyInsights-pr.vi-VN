---
title: 0x8004de40 khởi chạy công cụ OneDrive
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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946601"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 khởi chạy công cụ OneDrive

Nếu bạn gặp lỗi khi **đăng 0x8004de40** nhập vào máy tính, OneDrive khởi động lại máy tính trong khi kết nối với miền cơ quan hoặc trường học của bạn. Nếu bạn gặp lỗi này sau khi khởi động lại, hãy thử cách này trong khi kết nối với miền cơ quan hoặc trường học của bạn:

1. Bấm vào Bắt đầu và nhập **cmd** **hoặc**  dấu nhắc lệnh vào hộp tìm kiếm, bấm chuột phải vào ứng dụng dấu nhắc lệnh, rồi chọn Chạy với tư cách người  **quản trị**. Nếu bạn được nhắc nhập mật khẩu người quản trị hoặc xác nhận, hãy nhập mật khẩu hoặc bấm Cho **phép.**  

2. Trong cửa sổ Dấu nhắc Lệnh, **nhập dsregcmd /leave**  và chờ lệnh hoàn tất. Sau đó **nhập dsregcmd /join** và chờ lệnh hoàn tất.
3. Khởi động lại máy tính của bạn.
