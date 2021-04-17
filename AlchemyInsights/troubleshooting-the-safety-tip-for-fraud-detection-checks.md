---
title: Khắc phục sự cố Mẹo phát hiện gian lận
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834753"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Khắc phục sự cố Mẹo phát hiện gian lận

Nếu bạn nhận được Mẹo an toàn cho biết "người gửi không thể kiểm tra phát hiện gian lận của chúng tôi và có thể không phải người mà họ xuất hiện là", thì người gửi không thể vượt qua hoặc kiểm tra xác thực SPF. Phương pháp tốt nhất để giải quyết điều này là dành cho người gửi để ủy quyền cho mình. Nếu người gửi đang gửi thay mặt cho bạn, bạn cần phải ủy quyền cho họ bằng cách thêm địa chỉ IP của người gửi vào bản ghi SPF của bạn.
  
Xem [khắc phục sự cố Mẹo an toàn màu đỏ (đáng ngờ) để kiểm tra việc phát hiện gian lận](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) để biết thêm thông tin.
  
Dưới đây là một số liên kết khác có thể trợ giúp:
  
- [Cách Microsoft sử dụng khung chính sách người gửi (SPF) để ngăn chặn thư giả mạo](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Thiết lập SPF để giúp ngăn chặn giả mạo](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
