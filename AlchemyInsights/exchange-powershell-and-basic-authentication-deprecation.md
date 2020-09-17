---
title: Exchange PowerShell và tính năng xác thực cơ bản
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: f4f0f63112d639101ea9e9d7e9a9c16a32de4cf3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47782997"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="4b792-102">Exchange PowerShell và tính năng xác thực cơ bản</span><span class="sxs-lookup"><span data-stu-id="4b792-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="4b792-103">Để biết thông tin mới nhất về cách kết nối với Exchange Online PowerShell mà không cần phải sử dụng xác thực cơ bản, [vui lòng đến đây](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="4b792-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="4b792-104">Mô-đun PowerShell v2 sẽ không dùng xác thực cơ bản.</span><span class="sxs-lookup"><span data-stu-id="4b792-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="4b792-105">Xin lưu ý rằng xác thực cơ bản vẫn cần được kích hoạt trên máy khách của bạn.</span><span class="sxs-lookup"><span data-stu-id="4b792-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="4b792-106">Mô-đun PowerShell mới v2 dùng Auth hiện đại để thiết lập kết nối cho việc cho phép tất cả các lệnh ghép ngắn v2 dựa trên phần còn lại.</span><span class="sxs-lookup"><span data-stu-id="4b792-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="4b792-107">Ngoài các lệnh ghép ngắn v2, nó cũng cho phép bạn truy nhập các lệnh ghép ngắn PowerShell từ xa cũ hơn (RPS), yêu cầu phải được thiết lập phiên làm việc PowerShell từ xa.</span><span class="sxs-lookup"><span data-stu-id="4b792-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="4b792-108">Thiết lập một phiên RPS trên Windows Machine yêu cầu WinRM BasicAuth được kích hoạt trên máy khách ngay cả khi mô-đun sử dụng cơ chế xác thực hiện đại để xác thực dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="4b792-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="4b792-109">Đường ống WinRM cơ bản được sử dụng để vận chuyển các thẻ xác thực hiện đại.</span><span class="sxs-lookup"><span data-stu-id="4b792-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="4b792-110">Nếu WinRM cơ bản được tắt trên máy khách, các lệnh ghép ngắn v2 mới sẽ tiếp tục làm việc (nhưng các lệnh ghép ngắn RPS cũ hơn sẽ không).</span><span class="sxs-lookup"><span data-stu-id="4b792-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
