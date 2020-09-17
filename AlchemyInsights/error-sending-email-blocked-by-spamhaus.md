---
title: Lỗi khi gửi email bị SpamHaus chặn
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783825"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Lỗi gửi email: máy chủ khách đã bị chặn bằng SpamHaus

Địa chỉ IP đã gửi thư nằm trong danh sách chặn thuộc sở hữu của [SpamHaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Các lý do bị truy nhập bởi SpamHaus bao gồm các tài khoản đã xâm phạm, các máy xâm phạm chia sẻ một địa chỉ IP công cộng và các chính sách nhà cung cấp dịch vụ Internet (ISP). Các bản sửa lỗi có thể là:
  
- Đối với các thư đã chặn trong đó bạn kiểm soát máy chủ email nguồn, bạn cần xác định nguyên nhân và loại bỏ khối từ trang web SpamHaus.

- Đối với các thư đã chặn trong đó địa chỉ IP nguồn thuộc về người khác, chủ sở hữu địa chỉ cần loại bỏ khối từ trang web SpamHaus. Nếu địa chỉ IP nằm trên danh sách khối chính sách (PBL), chủ sở hữu có thể gán địa chỉ IP tĩnh khác hoặc loại bỏ địa chỉ khỏi PBL.

- Đối với các thư gửi đi từ tên miền của bạn được kết nối với Microsoft, bạn có thể nhận được lỗi này nếu các thư được định tuyến thông qua dịch vụ của bên thứ 3. Bạn có thể sử dụng công cụ tra cứu WHOIS để tìm chủ sở hữu địa chỉ IP bị chặn.
