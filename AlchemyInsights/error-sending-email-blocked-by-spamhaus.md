---
title: Lỗi gửi thư điện tử bị chặn bởi SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a16c998d2f289ea2da52454819f6677c405381a1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29496775"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Lỗi gửi thư điện tử: khách hàng lưu trữ bị chặn bằng cách sử dụng Spamhaus

Địa chỉ IP gửi thư là một danh sách chặn thuộc sở hữu của [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Lý do bị chặn bởi Spamhaus bao gồm tài khoản bị xâm phạm, xâm nhập máy chia sẻ một địa chỉ IP công cộng, và các chính sách cung cấp dịch vụ Internet (ISP). Bản sửa lỗi có thể là:
  
- Chặn thư trong nước vào Office 365 mà bạn kiểm soát các máy chủ email mã nguồn, bạn cần phải xác định nguyên nhân gây ra và loại bỏ các khối từ trang web của Spamhaus.
    
- Chặn thư trong nước vào Office 365 mà nguồn IP địa chỉ thuộc về người khác, chủ sở hữu của địa chỉ nhu cầu để loại bỏ khối từ trang web của Spamhaus. Nếu địa chỉ IP vào danh sách chặn chính sách (PBL), chủ sở hữu có thể gán một địa chỉ IP tĩnh khác nhau hoặc xóa địa chỉ khỏi PBL.
    
- Chặn thư đi từ miền Office 365 của mình, bạn có thể nhận được lỗi này nếu thư được định tuyến thông qua một dịch vụ bên thứ 3. Bạn có thể sử dụng một công cụ tra cứu WHOIS để tìm chủ sở hữu địa chỉ IP bị chặn.
    

