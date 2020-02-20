---
title: Không thể thiết lập hoặc xem chính sách AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158583"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Không thể thiết lập hoặc xem chính sách AllowSelfServicePurchase

Khi cố gắng thiết lập hoặc xem chính sách AllowSelfServicePurchase, bạn nhận được thông báo lỗi sau:

*HandleError: không thể truy xuất chính sách sản phẩm với PolicyId ' AllowSelfServicePurchase ', ErrorMessage-kết nối cơ bản bị đóng: một lỗi không mong muốn xảy ra trên một gửi.*

Điều này có thể là do một phiên bản cũ hơn của Transport Layer Security (TLS). Để kết nối dịch vụ MSCommerce, bạn cần phải sử dụng TLS 1,2 hoặc cao hơn.  

Hãy thử các bước sau để bật/đặt giao thức TLS 1,2, xác minh và thử lại.
 1. Tại dấu nhắc lệnh PowerShell (PS C:\) nhập lệnh sau để đặt giao thức TLS phiên bản 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Kiểm tra giao thức TLS (s) sử dụng, với các lệnh sau:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Thử lại lệnh nhận hoặc Cập Nhật khi cần thiết.

