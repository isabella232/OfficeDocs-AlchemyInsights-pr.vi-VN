---
title: 1554 Winsock lỗi 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903142"
---
# <a name="winsock-error-10061"></a>Winsock lỗi 10061

Mã lỗi này có nghĩa rằng Office 365 không thể thiết lập một cổng TCP (kết nối) với máy chủ mục tiêu. Nguyên nhân có thể nhất của lỗi này là một vấn đề với cấu hình tường lửa của bạn. Để khắc phục vấn đề, hãy kiểm tra các cài đặt này:
  
- Xác minh cấu hình tường lửa của bạn với các thông tin trong [Office 365 URL và dải địa chỉ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Nếu lỗi cụ thể để bảo vệ trực tuyến trao đổi (EOP), bạn nên đã được trước đó thông báo để thay đổi [địa chỉ IP bảo vệ trực tuyến trao đổi](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Xác minh rằng nhà cung cấp dịch vụ Internet (ISP) không phải là chặn cổng.
    
- Xác minh các thông minh chủ và mục tiêu máy chủ cài đặt kết nối của bạn.
    
Lưu ý rằng Office 365 không chặn *các* kết nối theo cách này. 
  

