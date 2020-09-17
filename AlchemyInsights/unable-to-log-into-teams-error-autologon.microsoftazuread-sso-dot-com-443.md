---
title: Không thể đăng nhập vào các nhóm do lỗi autologon.microsoftazuread-sso.com:443
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
ms.openlocfilehash: 649124db135805d8101b43dbead63860d36853ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799982"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Không thể đăng nhập vào các nhóm do lỗi tự động đăng nhập. microsoftazuread-SSO dot com: 443

Nếu SSO seamless được bật là xác thực O365, URL "autologon.microsoftazuread-sso.com" có thể cần phải được thêm vào site intranet.  Nếu trước đó đã được thêm vào các site tin cậy và SSO được dàn lại đang được sử dụng, nó sẽ được loại bỏ khỏi các trang tin cậy.

Vui lòng xem xét [danh sách khắc phục sự cố SSO liền mạch](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Làm theo các bước sau để thêm URL vào danh sách site intranet:

1. Mở Internet Explorer bằng cách bấm vào nút **bắt đầu** . Trong hộp tìm kiếm, nhập Internet Explorer, sau đó trong danh sách kết quả, hãy bấm **Internet Explorer**.
2. Bấm vào **công cụ**, rồi bấm **tùy chọn Internet**.
3. Bấm vào tab **bảo mật** .
4. Bây giờ, hãy bấm vào **site intranet Cục bộ** , rồi bấm vào nút **site** rồi **nâng cao** .
5. Nhập URL của trang web, rồi bấm vào **Thêm**.
6. Khi bạn đã hoàn tất, hãy bấm **đóng**.

Để biết thêm thông tin, hãy xem [tài liệu về việc triển khai SSO trong suốt cho O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (bao gồm quy trình dựa trên chính sách để thêm URL vào site intranet trong bước 3).
