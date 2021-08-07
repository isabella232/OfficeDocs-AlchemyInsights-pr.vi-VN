---
title: Không thể đặt hoặc xem chính sách AllowSelfServicePurchase
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
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020214"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Không thể đặt hoặc xem chính sách AllowSelfServicePurchase

Khi tìm cách đặt hoặc xem chính sách AllowSelfServicePurchase, bạn nhận được thông báo lỗi sau đây:

*HandleError : Không thể truy xuất chính sách sản phẩm với PolicyId 'AllowSelfServicePurchase', ErrorMessage - Kết nối cơ sở đã bị đóng: Đã xảy ra lỗi ngoài dự kiến trong một lần gửi.*

Sự cố này có thể do phiên bản cũ hơn của Transport Layer Security (TLS). Để kết nối dịch vụ MSCommerce, bạn cần sử dụng TLS 1.2 trở lên.  

Hãy thử các bước sau để bật/đặt giao thức TLS thành 1.2, xác minh và thử lại.
 1. Tại dấu nhắc lệnh PowerShell (PS C: hãy nhập lệnh sau đây để đặt giao thức \) TLS thành phiên bản 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Xác minh (các) giao thức TLS đang được sử dụng, với lệnh sau đây:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Hãy thực hiện lại lệnh Tải hoặc Cập nhật nếu cần.

