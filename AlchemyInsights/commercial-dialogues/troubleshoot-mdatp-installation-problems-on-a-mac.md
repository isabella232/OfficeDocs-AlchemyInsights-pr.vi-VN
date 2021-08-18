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
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091112"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Khắc phục sự cố cài đặt MDATP trên máy Mac

Nếu cài đặt thủ công không thành công, trang **Tóm** tắt của trình hướng dẫn cài đặt sẽ hiển thị lỗi sau đây:

"Đã xảy ra lỗi trong quá trình cài đặt. Chương trình cài đặt đã gặp lỗi khiến quá trình cài đặt không thành công. Hãy liên hệ với nhà sản xuất phần mềm để được trợ giúp."

Đối với triển khai MDM, trang cũng sẽ hiển thị lỗi cài đặt chung.

Mặc dù chúng tôi không hiển thị các lỗi chính xác đối với người dùng cuối, chúng tôi vẫn duy trì một tệp nhật ký với tiến độ cài đặt trong **/Library/Logs/Microsoft/mdatp/install.log**. Mỗi phiên cài đặt sẽ thêm vào tệp nhật ký này. Để chỉ xuất phiên cài đặt gần nhất, sử dụng `sed` .

Để tìm hiểu thêm, xem mục Khắc [phục sự cố cài đặt cho ATP của Bộ bảo vệ Microsoft cho máy Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)
