---
title: SharePoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709092"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="a8d65-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="a8d65-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="a8d65-103">Làm việc với PowerShell hoặc script trong SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="a8d65-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="a8d65-104">Truy nhập các nối kết dưới đây để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="a8d65-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="a8d65-105">Bắt đầu với SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="a8d65-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="a8d65-106">Kết nối với SPO PowerShell với xác thực đa yếu tố (MFA)</span><span class="sxs-lookup"><span data-stu-id="a8d65-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="a8d65-107">Các [mẫu và thực hành SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) chứa một thư viện của các lệnh PowerShell cho phép bạn thực hiện các hành động quản lý phức tạp đối với SPO.</span><span class="sxs-lookup"><span data-stu-id="a8d65-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="a8d65-108">Nếu bạn đang gặp vấn đề khi kết nối với trình bao quản lý SPO, hãy đảm bảo rằng bạn đã cập nhật phiên bản mới nhất và thử [nhập lại mô-đun](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) bằng cách dùng *"nhập-mô-đun Microsoft. Online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="a8d65-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="a8d65-109">Nếu bạn đang tìm cách chạy script mô hình đối tượng máy khách, bạn sẽ cần có các [cấu phần ứng dụng khách SharePoint Online SDK](https://www.microsoft.com/download/details.aspx?id=42038) được cài đặt trên máy cục bộ của bạn.</span><span class="sxs-lookup"><span data-stu-id="a8d65-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="a8d65-110">Nếu bạn đang gặp sự cố khi chạy script từ PowerShell, bạn có thể muốn xem xét việc Chạy PowerShell với tư cách là người quản trị và thay đổi [chính sách thực hiện](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="a8d65-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>