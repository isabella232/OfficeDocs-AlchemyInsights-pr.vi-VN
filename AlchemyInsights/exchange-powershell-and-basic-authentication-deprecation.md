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
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015711"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="72841-102">Exchange PowerShell và sự phản kháng xác thực cơ bản</span><span class="sxs-lookup"><span data-stu-id="72841-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="72841-103">Để biết thông tin mới nhất về cách kết nối với Exchange Online PowerShell mà không cần sử dụng xác thực cơ bản, [vui lòng truy cập ở đây](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="72841-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="72841-104">Xin lưu ý rằng xác thực cơ bản vẫn cần phải được kích hoạt trên máy khách của bạn.</span><span class="sxs-lookup"><span data-stu-id="72841-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="72841-105">Mô-đun PowerShell v2 mới sử dụng hiện đại Auth để thiết lập kết nối cho phép tất cả các lệnh ghép ngắn v2 dựa trên phần còn lại.</span><span class="sxs-lookup"><span data-stu-id="72841-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="72841-106">Ngoài các lệnh ghép ngắn v2, nó cũng cho phép bạn truy cập các lệnh ghép ngắn PowerShell từ xa (RPS) cũ hơn yêu cầu phiên PowerShell từ xa được thiết lập.</span><span class="sxs-lookup"><span data-stu-id="72841-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="72841-107">Thiết lập một phiên RPS trên máy Windows yêu cầu WinRM BasicAuth được kích hoạt trên máy khách mặc dù mô-đun sử dụng cơ chế hiện đại Auth để xác thực dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="72841-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="72841-108">Đường ống WinRM cơ bản Auth được sử dụng để vận chuyển các token hiện đại Auth.</span><span class="sxs-lookup"><span data-stu-id="72841-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="72841-109">Nếu WinRM cơ bản Auth bị vô hiệu hoá trên máy khách, lệnh ghép ngắn v2 mới sẽ tiếp tục hoạt động (nhưng cũ RPS lệnh ghép ngắn sẽ không).</span><span class="sxs-lookup"><span data-stu-id="72841-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
