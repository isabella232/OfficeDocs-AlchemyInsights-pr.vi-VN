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
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314226"
---
# <a name="active-directory-not-syncing"></a>Active Directory không đồng bộ

Nếu bạn đang nhận được lỗi đồng bộ, như "không đồng bộ hóa gần đây" hoặc nhận thấy trạng thái đồng bộ hóa thư mục trong cổng thông tin quản trị Office cho biết "Đã đồng bộ lần cuối hơn 3 ngày trước", đó có thể là AADConnect có cài đặt không chính xác hoặc không đủ quyền để thực hiện đồng bộ.  

Việc cài đặt lại AADConnect bằng cách sử dụng cài đặt nhanh có thể nhanh chóng giải quyết được sự cố:

1. [Tải xuống phiên bản AADConnect mới nhất.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Làm theo hướng dẫn để cài đặt nhanh.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Kết nối được cài đặt vào Windows Server 2012 trở lên. Máy chủ này phải nối miền và có thể là bộ kiểm soát miền hoặc máy chủ thành viên. Để biết danh sách đầy đủ các yêu cầu và Kết nối điều kiện tiên quyết của Azure AD, hãy xem lại Điều kiện tiên quyết cho [Azure AD Kết nối.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Để biết thêm thông tin về tài khoản dịch vụ AADConnect, hãy [xem mục Azure AD Kết nối: Tài khoản và quyền.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
