---
title: Không thể đặt hoặc xem chính sách mua mua của allowselfservice
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
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826113"
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

