---
title: Teams lỗi 4c7
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
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049330"
---
# <a name="4c7-error-in-microsoft-teams"></a>Lỗi 4c7 trong Microsoft Teams

Lỗi này xảy ra vì Microsoft Teams yêu cầu Xác thực Forms. Khi bạn triển khai Dịch vụ Liên kết Active Directory (AD FS), Xác thực Forms không được bật cho mạng nội bộ theo mặc định. Nếu Windows xác thực Tích hợp không thành công, bạn sẽ được nhắc đăng nhập bằng cách sử dụng Xác thực Forms.

Để giải quyết sự cố này, hãy bật Xác thực Forms bằng cách sử dụng phần đính vào Bảng điều khiển Quản lý Microsoft AD FS (MMC) trên máy tính có bản sao cục bộ của Active Directory. Caranya sebagai berikut: 

1. Trong ngăn dẫn hướng, duyệt đến Chính **sách Xác thực**.
2. Bên dưới **Hành** động trong ngăn chi tiết, chọn Chỉnh **sửa xác thực chính toàn cầu**.
3. Trên tab **Mạng nội bộ,** chọn Xác **thực Biểu mẫu**.
4. Chọn **OK** (hoặc **Áp dụng**).