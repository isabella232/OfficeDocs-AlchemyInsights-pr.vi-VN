---
title: Cấu hình và mở rộng thời gian có mã thông báo
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917201"
---
# <a name="configure-and-extend-token-lifetimes"></a>Cấu hình và mở rộng thời gian có mã thông báo

Bạn có thể xác định tuổi thọ của truy nhập, SAML hoặc ID mã thông báo do Microsoft Identity Platform phát hành. Bạn có thể đặt các hạn token cho tất cả các ứng dụng trong tổ chức của mình, cho một ứng dụng nhiều đối tượng thuê (nhiều tổ chức) hoặc đối với một hiệu trưởng dịch vụ cụ thể trong tổ chức của bạn. Để biết thêm thông tin, hãy đọc các [hạn của mã](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)thông báo cấu hình.

Ví dụ, đọc [ví dụ về cách cấu hình hạn của token](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Để tìm hiểu cách đặt cấu hình tuổi thọ và tính tương thích của mã thông báo trong Azure Active Directory B2C (Azure AD B2C), hãy xem mục [đặt cấu hình thẻ trong Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

Bài viết [cấu hình hành vi phiên trong Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) mô tả các phương pháp đăng nhập đơn (SSO) được sử dụng trong AZURE AD B2C và giúp bạn chọn phương pháp SSO thích hợp nhất khi cấu hình chính sách của bạn.

**Các thẻ mới có bao lâu? Chúng hợp lệ trong bao lâu?**

Token hạn là 1 giờ và tuổi thọ của phiên là 24 giờ. Điều này có nghĩa là nếu không có yêu cầu nào được thực hiện trong 24 giờ, bạn sẽ cần phải đăng nhập lại trước khi yêu cầu mã thông báo mới.

> [!NOTE]
> Sau khi 30 tháng 5, 2020, không có đối tượng thuê mới sẽ có thể sử dụng chính sách Lifetime mã thông báo cấu hình để cấu hình phiên và làm mới các thẻ. Việc việc phản đối sẽ xảy ra trong vài tháng sau đó, nghĩa là chúng tôi sẽ ngừng tôn phục phiên làm việc hiện tại và làm mới các phiếu ghi điểm. Bạn vẫn có thể cấu hình Access hạn token sau khi deprecation.






