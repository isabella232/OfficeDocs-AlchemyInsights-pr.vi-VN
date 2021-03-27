---
title: Tự động đăng nhập vào Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398751"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Tự động đăng nhập vào Microsoft Edge

Microsoft Edge sử dụng tài khoản hệ điều hành mặc định để tự động đăng nhập vào người dùng theo cách cấu hình thiết bị của người dùng. 

Các kịch bản của từng kiểu cấu hình thiết bị và quy trình đăng nhập người dùng phụ thuộc của nó được mô tả dưới đây:

- **Thiết bị được kết hợp/đọc-J**: tùy chọn này có sẵn trên Windows 10, xuống mức Windows và các phiên bản máy chủ tương ứng. Người dùng được tự động đăng nhập bằng tài khoản Azure Active Directory (AD).
- **Thiết bị được nối tên miền**: tùy chọn này sẵn có trên Windows 10, xuống mức Windows và các phiên bản máy chủ tương ứng. Theo mặc định, người dùng có tài khoản miền không được tự động đăng nhập; để kích hoạt tính năng đăng nhập tự động cho họ, hãy sử dụng chính sách **ConfigureOnPremisesAccountAutoSignIn** . Để kích hoạt tính năng đăng nhập tự động cho người dùng bằng tài khoản Azure AD, hãy cân nhắc việc gia nhập kết hợp thiết bị của họ.
- **Tài khoản mặc định của hệ điều hành là tài khoản Microsoft**: tùy chọn này sẵn dùng trên Windows 10 RS3 (phiên bản 1709, bản dựng 10.0.16299) và các phiên bản mới hơn. Kịch bản dường như không xảy ra trên các thiết bị doanh nghiệp. Tuy nhiên, nếu tài khoản của hệ điều hành mặc định là tài khoản Microsoft, thì Microsoft Edge sẽ tự động đăng nhập vào người dùng bằng tài khoản Microsoft.
 
 
