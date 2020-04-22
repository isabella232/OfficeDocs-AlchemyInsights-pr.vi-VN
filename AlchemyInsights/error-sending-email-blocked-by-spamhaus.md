---
title: Lỗi gửi email bị chặn bởi SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714280"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Lỗi gửi email: máy chủ khách hàng bị chặn bằng cách sử dụng SpamHaus

Địa chỉ IP gửi thư là một danh sách chặn thuộc sở hữu của [SpamHaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Lý do bị chặn bởi SpamHaus bao gồm các tài khoản xâm phạm, Máy chia sẻ địa chỉ IP công cộng và chính sách nhà cung cấp dịch vụ Internet (ISP). Các bản sửa lỗi có thể là:
  
- Đối với các thư bị chặn đến nơi bạn kiểm soát máy chủ email nguồn, bạn cần phải xác định nguyên nhân và loại bỏ khối từ trang web SpamHaus.

- Đối với các thư đến bị chặn trong đó địa chỉ IP nguồn thuộc về người khác, chủ sở hữu địa chỉ cần loại bỏ khối từ trang web SpamHaus. Nếu địa chỉ IP nằm trong danh sách chặn chính sách (PBL), chủ sở hữu có thể gán địa chỉ IP tĩnh khác hoặc xoá địa chỉ khỏi PBL.

- Đối với các thư đi bị chặn từ miền của bạn kết nối với Microsoft, bạn có thể nhận được lỗi này nếu thư được định tuyến thông qua dịch vụ bên thứ ba. Bạn có thể sử dụng công cụ tra cứu WHOIS để tìm chủ sở hữu địa chỉ IP bị chặn.
