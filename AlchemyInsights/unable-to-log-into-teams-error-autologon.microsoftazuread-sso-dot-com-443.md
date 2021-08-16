---
title: Không thể đăng nhập vào Teams do lỗi autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038422"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Không thể đăng nhập vào Teams do lỗi autologon.microsoftazuread-sso dot com:443

Nếu Seamless SSO được bật là xác thực O365, URL "autologon.microsoftazuread-sso.com" có thể cần được thêm vào Site Mạng nội bộ.  Nếu trước đó, site này đã được thêm vào Site tin cậy và SSO Liền mạch đang được sử dụng thì site này sẽ bị loại bỏ khỏi Site tin cậy.

Vui lòng xem lại Danh sách kiểm tra Khắc phục sự cố Seamless [SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Làm theo các bước sau để thêm URL vào danh sách Site Mạng nội bộ:

1. Mở Internet Explorer bằng cách bấm vào **nút Bắt** đầu. Trong hộp tìm kiếm, nhập Internet Explorer, rồi trong danh sách kết quả, bấm **vào Internet Explorer.**
2. Bấm **Công cụ**, rồi bấm Tùy chọn **Internet**.
3. Bấm tab **Bảo** mật.
4. Bây giờ, bấm **vào site Mạng nội bộ Cục** bộ, rồi bấm vào nút **site,** rồi nút **Nâng** cao.
5. Nhập URL Website và bấm **Thêm.**
6. Khi bạn đã hoàn tất, bấm **vào Đóng.**

Để biết thêm thông tin, xem mục Tài liệu hướng dẫn triển khai [Seamless SSO cho O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (bao gồm quy trình dựa trên Chính sách để thêm URL vào Site Mạng nội bộ ở Bước 3).
