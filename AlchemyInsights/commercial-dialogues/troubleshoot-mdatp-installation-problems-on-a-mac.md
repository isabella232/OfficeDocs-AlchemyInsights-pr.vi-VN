---
title: Khắc phục sự cố cài đặt MDATP trên máy Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749763"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Khắc phục sự cố cài đặt MDATP trên máy Mac

Nếu cài đặt thủ công không thành công, trang **tóm tắt** của trình hướng dẫn cài đặt sẽ hiển thị lỗi sau:

Lỗi "đã xảy ra trong quá trình cài đặt. Trình cài đặt gặp phải lỗi khiến quá trình cài đặt không thành công. Liên hệ với nhà sản xuất phần mềm để được trợ giúp. "

Đối với triển khai MDM, trang sẽ hiển thị lỗi cài đặt chung.

Mặc dù chúng tôi không hiển thị các lỗi chính xác cho người dùng cuối, chúng tôi giữ một tệp nhật ký với tiến trình cài đặt, trong **/Library/logs/Microsoft/mdatp/install.log**. Mỗi phiên cài đặt sẽ nối vào tệp nhật ký này. Để chỉ ra phiên cài đặt cuối cùng, hãy sử dụng `sed` .

Để tìm hiểu thêm, hãy xem [khắc phục sự cố cài đặt cho Microsoft Defender ATP cho Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
