---
title: Khắc phục sự cố Mẹo an toàn để kiểm tra phát hiện gian lận
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759534"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Khắc phục sự cố Mẹo an toàn để kiểm tra phát hiện gian lận

Nếu bạn nhận được một Mẹo an toàn cho biết "người gửi đã không kiểm tra phát hiện gian lận của chúng tôi và có thể không phải là những người mà họ xuất hiện là", sau đó người gửi không thể vượt qua hoặc kiểm tra xác thực DKIM hoặc SPF. Phương pháp tốt nhất để giải quyết điều này là cho người gửi để cho phép mình. Nếu người gửi gửi thay mặt bạn, bạn cần phải ủy quyền cho họ bằng cách thêm địa chỉ IP của người gửi vào bản ghi SPF của bạn.
  
Xem [khắc phục sự cố Mẹo an toàn màu đỏ (đáng ngờ) để kiểm tra phát hiện gian lận để](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) biết thêm thông tin.
  
Dưới đây là một số liên kết khác có thể giúp:
  
- [Cách Microsoft sử dụng khung chính sách người gửi (SPF) để tránh giả mạo](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [Thiết lập SPF để giúp ngăn chặn giả mạo](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
