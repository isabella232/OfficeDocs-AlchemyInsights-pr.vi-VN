---
title: Không thể đặt hoặc xem chính sách mua mua của allowselfservice
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735221"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Không thể đặt hoặc xem chính sách mua mua của allowselfservice

Khi cố gắng đặt hoặc xem chính sách mua mua của Allowselfservice, bạn nhận được thông báo lỗi sau đây:

*HandleError: không thể truy xuất chính sách sản phẩm với nội dung mua ' AllowSelfServicePurchase ', ErrorMessage-kết nối cơ sở đã được đóng: một lỗi không mong muốn xảy ra khi gửi.*

Điều này có thể do một phiên bản cũ của bảo mật tầng giao thông (TLS). Để kết nối với dịch vụ MSCommerce, bạn cần phải sử dụng TLS 1,2 hoặc cao hơn.  

Hãy thử các bước sau đây để bật/đặt giao thức TLS sang 1,2, xác nhận và thử lại.
 1. Tại dấu nhắc lệnh PowerShell (PS C: \) nhập lệnh sau đây để đặt giao thức TLS sang phiên bản 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Xác minh (các) (các) (các) (các) (các) (các) (các) (các) giao thức

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Thử lại các lệnh tải xuống và Cập Nhật khi cần thiết.

