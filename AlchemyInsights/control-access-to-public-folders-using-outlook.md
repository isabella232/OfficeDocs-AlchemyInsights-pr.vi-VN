---
title: Kiểm soát quyền truy nhập vào các thư mục công cộng bằng Outlook
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
- "3500007"
- "3462"
ms.openlocfilehash: 4ef62fe8c9cc438c48ed8897a8b3385b15669cdc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47804007"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="125aa-102">Kiểm soát quyền truy nhập vào các thư mục công cộng bằng Outlook</span><span class="sxs-lookup"><span data-stu-id="125aa-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="125aa-103">Để điều khiển người dùng có thể truy nhập vào các thư mục công cộng bằng cách dùng Outlook:</span><span class="sxs-lookup"><span data-stu-id="125aa-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="125aa-104">Sử dụng `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="125aa-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="125aa-105">$true: cho phép người dùng truy nhập các thư mục công cộng trong Outlook</span><span class="sxs-lookup"><span data-stu-id="125aa-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="125aa-106">$false: ngăn chặn quyền truy nhập của người dùng vào các thư mục công cộng trong Outlook.</span><span class="sxs-lookup"><span data-stu-id="125aa-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="125aa-107">Đây là giá trị mặc định.</span><span class="sxs-lookup"><span data-stu-id="125aa-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="125aa-108">Lưu ý: quy trình này chỉ có thể điều khiển kết nối với Outlook trên máy tính cho máy khách chạy Windows.</span><span class="sxs-lookup"><span data-stu-id="125aa-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="125aa-109">Người dùng có thể tiếp tục truy nhập vào các thư mục công cộng bằng OWA hoặc Outlook for Mac.</span><span class="sxs-lookup"><span data-stu-id="125aa-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="125aa-110">Để biết thêm thông tin, hãy xem [kiểm soát kết nối đến các thư mục công cộng trong Outlook](https://aka.ms/controlpf) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="125aa-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
