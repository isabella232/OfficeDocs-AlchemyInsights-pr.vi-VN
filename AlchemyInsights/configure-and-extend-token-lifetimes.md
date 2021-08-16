---
title: Đặt cấu hình và mở rộng thời hạn mã thông báo
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
ms.openlocfilehash: 97e89feda45439dae59acca5817fdf359623d647997d08a5cbe4a6314fa6db3a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044938"
---
# <a name="configure-and-extend-token-lifetimes"></a>Đặt cấu hình và mở rộng thời hạn mã thông báo

Bạn có thể chỉ định thời hạn của mã thông báo truy nhập, SAML hoặc ID do người phát hành Nền tảng định danh Microsoft. Bạn có thể đặt thời hạn mã thông báo cho tất cả các ứng dụng trong tổ chức của bạn, cho ứng dụng nhiều đối tượng thuê (nhiều tổ chức) hoặc cho một dịch vụ chính cụ thể trong tổ chức của bạn. Để biết thêm thông tin, hãy [đọc thời hạn mã thông báo có thể cấu hình.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

Ví dụ: đọc các ví [dụ về cách cấu hình thời hạn mã thông báo](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Để tìm hiểu cách đặt cấu hình tuổi thọ và tính tương thích của mã thông báo trong Azure Active Directory B2C (Azure AD B2C), hãy xem đặt cấu hình mã thông báo [trong Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

Bài viết Đặt cấu hình hành vi phiên trong [Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) mô tả các phương pháp đăng nhập đơn (SSO) được sử dụng trong Azure AD B2C và giúp bạn chọn phương pháp SSO phù hợp nhất khi đặt cấu hình chính sách của mình.

**Các mã thông báo sẽ kéo dài bao lâu? Chúng hợp lệ trong bao lâu?**

Thời hạn của mã thông báo là 1 giờ và thời hạn phiên là 24 giờ. Điều này nghĩa là nếu không có yêu cầu nào được thực hiện trong 24 giờ, bạn sẽ cần phải đăng nhập lại trước khi yêu cầu mã thông báo mới.

> [!NOTE]
> Sau ngày 30 tháng 5 năm 2020, không có đối tượng thuê mới nào có thể sử dụng chính sách Thời hạn mã thông báo có thể cấu hình để đặt cấu hình phiên và làm mới mã thông báo. Việc ngừng phát hành sẽ xảy ra trong vòng vài tháng sau đó, điều này có nghĩa là chúng tôi sẽ ngừng thực hiện phiên hiện có và làm mới mã thông báo. Bạn vẫn có thể đặt cấu hình thời hạn mã thông báo truy nhập sau khi không còn sử dụng.






