---
title: Lỗi gửi email bị SpamHaus chặn
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
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8372032e19bd2ebaf3ba8cc8e87f19ef3e2edf1e607b1739a919f6dcc443cd97
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946816"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Lỗi gửi email: Máy chủ khách đã bị chặn bằng Spamhaus

Địa chỉ IP đã gửi thư nằm trong danh sách chặn của [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Các lý do để Spamhaus chặn bao gồm tài khoản bị xâm phạm, máy bị xâm phạm dùng chung địa chỉ IP công cộng và chính sách Nhà cung cấp Dịch vụ Internet (ISP). Cách khắc phục khả thi:
  
- Đối với các thư đến bị chặn mà bạn kiểm soát máy chủ email nguồn, bạn cần xác định nguyên nhân và loại bỏ việc chặn khỏi website Spamhaus.

- Đối với các thư đến bị chặn có địa chỉ IP nguồn thuộc về người khác, chủ sở hữu địa chỉ đó cần loại bỏ việc chặn khỏi website Spamhaus. Nếu địa chỉ IP nằm trên Danh sách Chặn Chính sách (PBL), chủ sở hữu có thể gán một địa chỉ IP tĩnh khác hoặc loại bỏ địa chỉ khỏi PBL.

- Đối với các thư đi bị chặn do miền của bạn kết nối với Microsoft, bạn có thể nhận được lỗi này nếu thư được định tuyến thông qua dịch vụ của bên thứ 3. Bạn có thể sử dụng công cụ tra cứu WHOIS để tìm chủ sở hữu địa chỉ IP bị chặn.
