---
title: Exchange PowerShell và sự phản kháng xác thực cơ bản
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: a0f01d7ecaa444777aa0675795e588790ab22f19
ms.sourcegitcommit: 9e44b852d18a2816acac0aacb78cb99b4c114368
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/22/2020
ms.locfileid: "45205217"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="7af3c-102">Exchange PowerShell và sự phản kháng xác thực cơ bản</span><span class="sxs-lookup"><span data-stu-id="7af3c-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="7af3c-103">Để biết thông tin mới nhất về cách kết nối với Exchange Online PowerShell mà không cần sử dụng xác thực cơ bản, [vui lòng truy cập ở đây](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="7af3c-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="7af3c-104">Mô-đun PowerShell v2 không sử dụng xác thực cơ bản.</span><span class="sxs-lookup"><span data-stu-id="7af3c-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="7af3c-105">Xin lưu ý rằng xác thực cơ bản vẫn cần phải được kích hoạt trên máy khách của bạn.</span><span class="sxs-lookup"><span data-stu-id="7af3c-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="7af3c-106">Mô-đun PowerShell v2 mới sử dụng hiện đại Auth để thiết lập kết nối cho phép tất cả các lệnh ghép ngắn v2 dựa trên phần còn lại.</span><span class="sxs-lookup"><span data-stu-id="7af3c-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="7af3c-107">Ngoài các lệnh ghép ngắn v2, nó cũng cho phép bạn truy cập các lệnh ghép ngắn PowerShell từ xa (RPS) cũ hơn yêu cầu phiên PowerShell từ xa được thiết lập.</span><span class="sxs-lookup"><span data-stu-id="7af3c-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="7af3c-108">Thiết lập một phiên RPS trên máy Windows yêu cầu WinRM BasicAuth được kích hoạt trên máy khách mặc dù mô-đun sử dụng cơ chế hiện đại Auth để xác thực dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="7af3c-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="7af3c-109">Đường ống WinRM cơ bản Auth được sử dụng để vận chuyển các token hiện đại Auth.</span><span class="sxs-lookup"><span data-stu-id="7af3c-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="7af3c-110">Nếu WinRM cơ bản Auth bị vô hiệu hoá trên máy khách, lệnh ghép ngắn v2 mới sẽ tiếp tục hoạt động (nhưng cũ RPS lệnh ghép ngắn sẽ không).</span><span class="sxs-lookup"><span data-stu-id="7af3c-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
