---
title: SharePoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786911"
---
# <a name="sharepoint-online-powershell"></a>SharePoint Online PowerShell

Làm việc với PowerShell hoặc script trong SharePoint Online? Truy nhập các nối kết dưới đây để biết thêm thông tin.
- [Bắt đầu với SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Kết nối với SPO PowerShell với xác thực đa yếu tố (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- Các [mẫu và thực hành SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) chứa một thư viện của các lệnh PowerShell cho phép bạn thực hiện các hành động quản lý phức tạp đối với SPO.

> [!NOTE]
> - Nếu bạn đang gặp vấn đề khi kết nối với trình bao quản lý SPO, hãy đảm bảo rằng bạn đã cập nhật phiên bản mới nhất và thử [nhập lại mô-đun](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) bằng cách dùng *"nhập-mô-đun Microsoft. Online. SharePoint. PowerShell".*
> - Nếu bạn đang tìm cách chạy script mô hình đối tượng máy khách, bạn sẽ cần có các [cấu phần ứng dụng khách SharePoint Online SDK](https://www.microsoft.com/download/details.aspx?id=42038) được cài đặt trên máy cục bộ của bạn.
> - Nếu bạn đang gặp sự cố khi chạy script từ PowerShell, bạn có thể muốn xem xét việc Chạy PowerShell với tư cách là người quản trị và thay đổi [chính sách thực hiện](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).