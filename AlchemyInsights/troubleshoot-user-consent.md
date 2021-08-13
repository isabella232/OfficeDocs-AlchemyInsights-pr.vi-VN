---
title: Khắc phục sự cố về sự chấp thuận của người
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007920"
---
# <a name="troubleshoot-user-consent"></a>Khắc phục sự cố về sự chấp thuận của người

1. Bạn có thể đặt cấu hình cách người dùng cuối đồng ý với các ứng dụng thông qua Cổng thông tin Azure hoặc PowerShell. Xem cài [đặt Sự chấp thuận của người](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) dùng để biết thêm thông tin.
1. Người quản trị cũng có thể sử [dụng API Microsoft Graph để](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) cấp quyền được ủy quyền thay mặt cho một người dùng đơn lẻ. Để biết thêm thông tin, [hãy xem mục Nhận quyền truy nhập thay mặt người dùng.](https://docs.microsoft.com/graph/auth-v2-user)
1. [Lỗi Đồng ý của Người](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)dùng : bài viết này thảo luận về các lỗi có thể xảy ra trong quá trình chấp thuận ứng dụng. Nếu bạn đang khắc phục sự cố lời nhắc chấp thuận ngoài dự tính mà không chứa bất kỳ thông báo lỗi nào, hãy xem [Kịch bản xác thực cho Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).