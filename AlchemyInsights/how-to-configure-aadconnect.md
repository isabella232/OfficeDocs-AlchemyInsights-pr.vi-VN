---
title: 646 Cách đặt cấu hình AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963665"
---
# <a name="configure-sync-features"></a>Cấu hình các tính năng đồng bộ

Azure AD Kết nối bao gồm một số tính năng được bật theo mặc định hoặc bạn có thể bật sau. Một số tính năng yêu cầu cấu hình bổ sung trong các môi trường cụ thể.

- [Lọc giới hạn](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) các đối tượng được đồng bộ hóa với Azure AD. Theo mặc định, tất cả người dùng, liên hệ, nhóm và tài khoản Windows 10 tính của bạn đều được đồng bộ hóa. Bạn có thể bao gồm hoặc loại trừ các đối tượng dựa trên tên miền, OU hoặc các thuộc tính khác.

- [Đồng bộ hóa băm mật khẩu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) đồng bộ hóa băm mật khẩu từ Active Directory tại chỗ với Azure AD. Điều này cho phép quản lý mật khẩu ở một vị trí, nhưng sử dụng cùng một mật khẩu trong cả môi trường tại chỗ và trên đám mây. Vì Active Directory là nguồn có thẩm quyền, bạn có thể dùng chính sách mật khẩu của riêng bạn.

- Đặt lại mật khẩu tự phục vụ [(SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) cho phép người dùng đặt lại mật khẩu của riêng mình trong đám mây trong khi vẫn áp dụng chính sách mật khẩu tại chỗ của bạn.

- [Ghi lại thiết bị](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) cho phép ghi lại các thiết bị đã đăng ký trong Azure AD vào Active Directory tại chỗ để có thể sử dụng các thiết bị này để truy nhập có điều kiện.

- [Ngăn chặn việc xóa ngẫu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) nhiên được bật theo mặc định để giúp ngăn chặn quá nhiều việc xóa đối tượng đồng thời (hơn 500 đối tượng cho mỗi quá trình đồng bộ). Bạn có thể thay đổi thiết đặt này để đáp ứng nhu cầu của tổ chức bạn.

- [Tính năng tự động](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) nâng cấp được bật theo mặc định cho các bản cài đặt nhanh và giúp đảm bảo phiên bản Azure AD Kết nối luôn cập nhật.
