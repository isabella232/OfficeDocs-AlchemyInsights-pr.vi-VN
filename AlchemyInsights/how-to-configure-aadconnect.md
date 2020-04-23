---
title: 646 làm thế nào để cấu hình AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722588"
---
# <a name="configure-sync-features"></a>Cấu hình tính năng đồng bộ

Azure AD kết nối bao gồm một số tính năng được kích hoạt theo mặc định, hoặc bạn có thể kích hoạt sau. Một số tính năng yêu cầu cấu hình bổ sung trong môi trường cụ thể.

- [Lọc](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) giới hạn các đối tượng được đồng bộ hoá Azure AD. Theo mặc định, tất cả người dùng, danh bạ, nhóm và tài khoản máy tính Windows 10 được đồng bộ hoá. Bạn có thể bao gồm hoặc loại trừ các đối tượng dựa trên miền, OUs hoặc các thuộc tính khác.

- [Mật khẩu băm đồng bộ hóa](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) mật khẩu băm từ Active Directory tại chỗ sang Azure AD. Điều này cho phép quản lý mật khẩu tại một địa chỉ, nhưng sử dụng cùng một mật khẩu trong môi trường tại chỗ và đám mây. Vì Active Directory là nguồn có thẩm quyền, bạn có thể sử dụng chính sách mật khẩu của riêng bạn.

- [Tự dịch vụ đặt lại mật khẩu (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) cho phép người dùng đặt lại mật khẩu của riêng mình trong đám mây trong khi vẫn áp dụng chính sách mật khẩu tại chỗ của bạn.

- [Thiết bị](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) ghi lại cho phép các thiết bị đăng ký trong Azure AD được viết trở lại Active Directory tại chỗ để họ có thể được sử dụng để truy cập có điều kiện.

- [Ngăn chặn tình cờ xóa](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) được kích hoạt theo mặc định để giúp ngăn chặn quá nhiều xoá đối tượng đồng thời (hơn 500 đối tượng cho mỗi đồng bộ hóa). Bạn có thể thay đổi cài đặt này để đáp ứng nhu cầu của tổ chức của bạn.

- [Tự động nâng cấp](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) được bật theo mặc định cho các cài đặt nhanh và giúp đảm bảo Phiên bản Azure AD kết nối luôn là hiện tại.
