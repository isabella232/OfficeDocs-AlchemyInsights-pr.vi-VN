---
title: Khắc phục sự cố người dùng
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
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901624"
---
# <a name="troubleshoot-user-consent"></a>Khắc phục sự cố người dùng

1. Bạn có thể cấu hình cách thức người dùng cuối đồng ý với các ứng dụng thông qua Azure Portal hoặc PowerShell. Xem [thiết đặt chấp thuận của người dùng](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) để biết thêm thông tin.
1. Người quản trị cũng có thể sử dụng [API của Microsoft graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) để cấp sự đồng ý cho phép ủy quyền thay mặt cho một người dùng duy nhất. Để biết thêm thông tin, hãy xem [nhận quyền truy nhập thay mặt cho người dùng](https://docs.microsoft.com/graph/auth-v2-user).
1. [Lỗi người dùng chấp thuận](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): bài viết này thảo luận về các lỗi có thể xảy ra trong quá trình đồng ý với một ứng dụng. Nếu bạn đang khắc phục sự cố không mong đợi lời nhắc không chứa bất kỳ thông báo lỗi nào, hãy xem [kịch bản xác thực cho AZURE AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).