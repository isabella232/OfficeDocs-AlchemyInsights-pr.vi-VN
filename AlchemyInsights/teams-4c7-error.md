---
title: Lỗi nhóm 6c 7
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
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786691"
---
# <a name="4c7-error-in-microsoft-teams"></a>lỗi 6x7 trong Microsoft nhóm

Lỗi này xảy ra vì Microsoft nhóm yêu cầu xác thực biểu mẫu. Khi bạn triển khai các dịch vụ liên kết Active Directory (AD FS), xác thực biểu mẫu không được kích hoạt cho mạng nội bộ theo mặc định. Nếu xác thực tích hợp Windows không thành công, bạn sẽ được nhắc đăng nhập bằng cách sử dụng xác thực biểu mẫu.

Để giải quyết sự cố này, hãy bật xác thực biểu mẫu bằng cách sử dụng trình điều khiển Microsoft Management Console (MMC) của AD FS trên máy tính có bản sao cục bộ của Active Directory. Caranya sebagai berikut: 

1. Trong ngăn dẫn hướng, duyệt đến **chính sách xác thực**.
2. Bên dưới **hành động** trong ngăn chi tiết, hãy chọn **chỉnh sửa xác thực toàn cầu chính**.
3. Trên tab **intranet** , chọn **biểu mẫu xác thực**.
4. Chọn **OK** (hoặc **áp dụng**).