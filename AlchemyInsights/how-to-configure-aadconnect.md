---
title: 646 cách đặt cấu hình cho kết nối
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
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704511"
---
# <a name="configure-sync-features"></a>Đặt cấu hình các tính năng đồng bộ

Azure AD Connect bao gồm một số tính năng được bật theo mặc định, hoặc bạn có thể bật sau này. Một số tính năng yêu cầu cấu hình bổ sung trong các môi trường cụ thể.

- [Lọc](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) giới hạn đối tượng được đồng bộ hóa với Azure AD. Theo mặc định, tất cả người dùng, liên hệ, nhóm và tài khoản máy tính chạy Windows 10 đều được đồng bộ. Bạn có thể bao gồm hoặc loại trừ các đối tượng dựa trên tên miền, dữ hoặc thuộc tính khác.

- [Đồng bộ hóa hash mật khẩu đồng bộ hóa](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) băm mật khẩu từ Active Directory tại chỗ vào Azure AD. Điều này cho phép quản lý mật khẩu ở một vị trí, nhưng sử dụng cùng một mật khẩu trong cả môi trường trên nền tảng tại cơ sở và điện toán đám mây. Vì Active Directory là nguồn có thẩm quyền, bạn có thể sử dụng chính sách mật khẩu của riêng bạn.

- [Đặt lại mật khẩu tự phục vụ (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) cho phép người dùng đặt lại mật khẩu của riêng mình trong nền tảng điện toán đám mây trong khi vẫn áp dụng chính sách mật khẩu tại cơ sở của bạn.

- [Writeback thiết bị](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) cho phép các thiết bị đã đăng ký trong Azure AD được ghi lại vào Active Directory tại chỗ để chúng có thể sử dụng cho Access có điều kiện.

- [Tránh xóa bỏ tình cờ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) được bật theo mặc định để giúp ngăn không cho quá nhiều đối tượng đồng thời (hơn 500 đối tượng đồng bộ). Bạn có thể thay đổi thiết đặt này để đáp ứng nhu cầu của tổ chức của mình.

- Tính năng [nâng cấp tự động](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) được bật theo mặc định cho việc cài đặt hiện tại và giúp đảm bảo Phiên bản của bạn kết nối Azure AD luôn là hiện tại.
