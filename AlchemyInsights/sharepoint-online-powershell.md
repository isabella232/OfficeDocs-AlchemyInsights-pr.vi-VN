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
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="81050-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="81050-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="81050-103">Làm việc với PowerShell hoặc script trong SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="81050-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="81050-104">Truy nhập các nối kết dưới đây để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="81050-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="81050-105">Bắt đầu với SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="81050-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="81050-106">Kết nối với SPO PowerShell với xác thực đa yếu tố (MFA)</span><span class="sxs-lookup"><span data-stu-id="81050-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="81050-107">Các [mẫu và thực hành SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) chứa một thư viện của các lệnh PowerShell cho phép bạn thực hiện các hành động quản lý phức tạp đối với SPO.</span><span class="sxs-lookup"><span data-stu-id="81050-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="81050-108">Nếu bạn đang gặp vấn đề khi kết nối với trình bao quản lý SPO, hãy đảm bảo rằng bạn đã cập nhật phiên bản mới nhất và thử [nhập lại mô-đun](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) bằng cách dùng *"nhập-mô-đun Microsoft. Online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="81050-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="81050-109">Nếu bạn đang tìm cách chạy script mô hình đối tượng máy khách, bạn sẽ cần có các [cấu phần ứng dụng khách SharePoint Online SDK](https://www.microsoft.com/download/details.aspx?id=42038) được cài đặt trên máy cục bộ của bạn.</span><span class="sxs-lookup"><span data-stu-id="81050-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="81050-110">Nếu bạn đang gặp sự cố khi chạy script từ PowerShell, bạn có thể muốn xem xét việc Chạy PowerShell với tư cách là người quản trị và thay đổi [chính sách thực hiện](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="81050-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>