---
title: Khắc phục sự cố về mẹo về an toàn tra phát hiện gian lận
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
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955988"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Khắc phục sự cố về mẹo về an toàn tra phát hiện gian lận

Nếu bạn đang gặp thông báo mẹo về an toàn rằng "Người gửi đã không thực hiện kiểm tra phát hiện gian lận của chúng tôi và có thể không phải là người có vẻ là người đó", thì người gửi đã không vượt qua được kiểm tra xác thực của DKIM hoặc SPF. Phương pháp tốt nhất để giải quyết điều này là để người gửi tự ủy quyền. Nếu người gửi đang gửi thay mặt bạn, bạn cần ủy quyền cho họ bằng cách thêm địa chỉ IP của người gửi vào bản ghi SPF của bạn.
  
Xem [khắc phục sự cố màu đỏ (đáng ngờ) mẹo về an toàn tra tìm kiếm gian lận để](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) biết thêm thông tin.
  
Dưới đây là một số liên kết khác có thể giúp ích:
  
- [Cách Microsoft sử dụng khung chính sách người gửi (SPF) để ngăn chặn giả mạo](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Thiết lập SPF để giúp ngăn chặn giả mạo](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
