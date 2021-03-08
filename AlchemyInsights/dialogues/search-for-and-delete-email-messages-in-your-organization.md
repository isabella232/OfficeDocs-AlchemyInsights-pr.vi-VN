---
title: Tìm kiếm và xóa thông điệp email trong tổ chức của bạn
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527276"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Tìm kiếm và xóa thông điệp email trong tổ chức của bạn

Làm theo các bước sau đây:

1. Nếu bạn không phải là người quản trị toàn cầu, để tìm kiếm thư tài khoản của bạn phải được thêm vào **nhóm vai trò trình quản lý Ekhám phá** hoặc **vai trò quản lý tìm kiếm tuân thủ**. Để xóa thư, bạn sẽ cần phải tham gia vào **nhóm vai trò quản lý tổ chức** hoặc **vai trò tìm kiếm và dọn sạch quản lý**. Quyền đối với các vai trò này được gán trong [Trung tâm tuân thủ & bảo mật.](https://protection.office.com)
2. [Tạo một tìm kiếm nội dung](https://docs.microsoft.com/office365/securitycompliance/content-search) để tìm thư cần xóa.
3. [Kết nối với Trung tâm bảo mật & PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Nếu bạn đang sử dụng MFA, hãy xem các hướng dẫn sau: [kết nối với Trung tâm bảo mật & PowerShell bằng cách dùng xác thực đa yếu tố](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Xóa bỏ thư: chạy `New-ComplianceSearchAction` lệnh ghép ngắn để xóa thư. Thư đã xóa được di chuyển đến thư mục các mục có thể phục hồi của người dùng. Đối với lệnh ví dụ, hãy xem [bước 3: xóa thư.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
