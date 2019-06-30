---
title: 646 làm thế nào để cấu hình AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 0569cb10c1d1dd422709de5d2569e43ee9d75386
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35385406"
---
# <a name="configure-sync-features"></a>Cấu hình tính năng đồng bộ hóa

Azure quảng cáo kết nối bao gồm một số tính năng đó được kích hoạt theo mặc định, hoặc bạn có thể kích hoạt sau đó. Một số tính năng yêu cầu cấu hình bổ sung trong môi trường cụ thể.

- Giới hạn [lọc](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) các đối tượng được đồng bộ hoá Azure quảng cáo. Theo mặc định, tất cả người dùng, số liên lạc, nhóm, và Windows 10 máy tính tài khoản được đồng bộ hoá. Bạn có thể bao gồm hoặc loại trừ các đối tượng dựa trên tên miền, Anh hoặc thuộc tính khác.

- [Mật khẩu băm đồng bộ hóa](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) đồng bộ hóa các hash mật khẩu từ Active Directory tại chỗ để quảng cáo Azure. Điều này cho phép quản lý mật khẩu ở một vị trí, nhưng sử dụng cùng một mật khẩu trong cả hai chỗ mây và môi trường. Vì hoạt động thư mục nguồn thẩm quyền, bạn có thể sử dụng chính sách mật khẩu của riêng bạn.

- [Đặt lại mật khẩu tự phục vụ (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) cho phép người dùng đặt lại mật khẩu của riêng của họ trong các đám mây trong khi vẫn còn áp dụng chính sách mật khẩu tại chỗ của bạn.

- [Thiết bị writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) cho phép đăng ký các thiết bị trong các quảng cáo Azure được viết lại để Active Directory tại chỗ để họ có thể được sử dụng để truy cập có điều kiện.

- [Ngăn chặn tình cờ xóa](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) được kích hoạt theo mặc định để giúp ngăn chặn quá nhiều đối tượng đồng thời xoá (hơn 500 đối tượng cho một đồng bộ hoá). Bạn có thể thay đổi cài đặt này để đáp ứng nhu cầu của tổ chức của bạn.

- [Nâng cấp tự động](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) được kích hoạt theo mặc định cho việc cài đặt nhận và giúp đảm bảo rằng các phiên bản của Azure quảng cáo kết nối luôn luôn là hiện tại.
