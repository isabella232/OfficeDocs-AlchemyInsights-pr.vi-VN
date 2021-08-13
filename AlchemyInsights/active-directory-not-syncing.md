---
title: Active Directory không đồng bộ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 4bfbe6b2dd9a2112f0cb7af0d6e7a46693bc70680895fd674ddb0332b7071797
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937123"
---
# <a name="active-directory-not-syncing"></a>Active Directory không đồng bộ

Nếu bạn đang nhận được lỗi đồng bộ, chẳng hạn như "không đồng bộ hóa gần đây" hoặc nhận thấy trạng thái đồng bộ hóa thư mục trong cổng thông tin quản trị Office cho biết "Đã đồng bộ lần cuối hơn 3 ngày trước", đó có thể là AADConnect có cài đặt không chính xác hoặc không đủ quyền để thực hiện đồng bộ.  

Việc cài đặt lại AADConnect bằng cách sử dụng cài đặt nhanh có thể giải quyết sự cố một cách nhanh chóng:

1. [Tải xuống phiên bản AADConnect mới nhất.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Làm theo hướng dẫn để cài đặt nhanh.](/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Kết nối được cài đặt trên Windows Server 2012 trở lên. Máy chủ này phải nối miền và có thể là bộ kiểm soát miền hoặc máy chủ thành viên. Để biết danh sách đầy đủ các yêu cầu và Kết nối điều kiện tiên quyết của Azure AD, hãy xem lại Điều kiện tiên quyết cho [Azure AD Kết nối.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Để biết thêm thông tin về tài khoản dịch vụ AADConnect, hãy [xem mục Azure AD Kết nối: Tài khoản và quyền.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)
