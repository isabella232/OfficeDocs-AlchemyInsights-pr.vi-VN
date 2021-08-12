---
title: Tìm kiếm và xóa thư email trong tổ chức của bạn
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
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948905"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Tìm kiếm và xóa thư email trong tổ chức của bạn

Làm theo các bước sau:

1. Nếu bạn không phải là người quản trị toàn cầu,  để tìm kiếm thư, tài khoản của bạn phải được thêm vào nhóm vai trò Người quản lý Khám phá Điện tử hoặc vai trò quản lý **Tìm kiếm Tuân thủ.** Để xóa thư, bạn sẽ cần tham gia nhóm vai trò **Quản lý Tổ chức hoặc** vai trò quản lý Tìm kiếm và Dọn **sạch**. Quyền đối với các vai trò này được gán trong [Trung tâm Bảo & tuân thủ.](https://protection.office.com)
2. [Tạo một tìm kiếm nội](https://docs.microsoft.com/office365/securitycompliance/content-search) dung để tìm thư cần xóa.
3. [Kết nối tâm Bảo mật & Tuân thủ PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Nếu bạn đang sử dụng MFA, hãy xem các hướng dẫn sau: Cách Kết nối trung tâm Bảo mật & Tuân thủ [PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell) bằng cách sử dụng xác thực đa yếu tố
4. Xóa thông báo: chạy `New-ComplianceSearchAction` lệnh ghép ngắn để xóa thư. Thư đã xóa được chuyển vào thư mục Các mục Có thể khôi phục của người dùng. Để biết lệnh ví dụ, hãy [xem Bước 3: Xóa thư.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
