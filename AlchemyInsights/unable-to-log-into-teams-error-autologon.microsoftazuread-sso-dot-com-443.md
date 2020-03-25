---
title: Không thể đăng nhập vào teams do lỗi autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932283"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Không thể đăng nhập vào nhóm do lỗi tự động đăng nhập. microsoftazuread-SSO dot com: 443

Nếu liền mạch SSO được kích hoạt như xác thực O365, URL "autologon.microsoftazuread-sso.com" có thể cần phải được thêm vào trang web intranet.  Nếu nó đã được thêm vào site tin cậy và liền mạch SSO đang được sử dụng, nó sẽ bị xoá khỏi site tin cậy.

Vui lòng đánh giá [danh sách kiểm tra khắc phục sự cố SSO liền mạch](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Hãy làm theo các bước sau để thêm URL vào danh sách site intranet:

1. Mở Internet Explorer bằng cách bấm vào nút **bắt đầu** . Trong hộp tìm kiếm, nhập Internet Explorer, sau đó, trong danh sách kết quả, bấm **Internet Explorer**.
2. Bấm **công cụ**, và sau đó bấm **tùy chọn Internet**.
3. Nhấp vào tab **bảo mật** .
4. Bây giờ bấm vào các **trang web Intranet Nội bộ** và sau đó bấm vào nút các **trang web** và sau đó **nâng cao** nút.
5. Nhập URL trang web và nhấp vào **Thêm**.
6. Khi bạn hoàn tất, bấm **đóng**.

Để biết thêm thông tin, xem [tài liệu để triển khai liền mạch SSO cho O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (bao gồm quy trình dựa trên chính sách để thêm URL vào trang web intranet trong bước 3).
