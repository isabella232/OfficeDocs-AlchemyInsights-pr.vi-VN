---
title: Lỗi teams 4c7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796472"
---
# <a name="4c7-error-in-microsoft-teams"></a>lỗi 4c7 trong Microsoft teams

Lỗi này xảy ra do Microsoft teams yêu cầu xác thực biểu mẫu. Khi bạn triển khai dịch vụ liên kết Active Directory (AD FS), hình thức xác thực không được kích hoạt cho mạng nội bộ theo mặc định. Nếu xác thực tích hợp Windows không thành công, bạn được nhắc đăng nhập bằng cách sử dụng xác thực biểu mẫu.

Để giải quyết vấn đề này, cho phép hình thức xác thực bằng cách sử dụng AD FS Microsoft Management Console (MMC) đính vào trên máy tính có bản sao cục bộ của Active Directory. Caranya sebagai berikut: 

1. Trong ngăn điều hướng, duyệt đến **chính sách xác thực**.
2. Trong **hành động** trong ngăn chi tiết, chọn **chỉnh sửa xác thực chính toàn cầu**.
3. Trên tab **intranet** , chọn **hình thức xác thực**.
4. Chọn **OK** (hoặc **áp dụng**).