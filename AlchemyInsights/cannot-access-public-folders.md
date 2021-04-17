---
title: Không thể truy nhập thư mục công cộng
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
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819534"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="71b41-102">Outlook không thể kết nối với các thư mục công cộng</span><span class="sxs-lookup"><span data-stu-id="71b41-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="71b41-103">Nếu quyền truy nhập thư mục công cộng không hoạt động với một số người dùng, hãy thử làm như sau:</span><span class="sxs-lookup"><span data-stu-id="71b41-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="71b41-104">Kết nối với EXO PowerShell và đặt cấu hình tham số DefaultPublicFolderMailbox trên tài khoản người dùng vấn đề để khớp với tham số trên tài khoản người dùng đang làm việc.</span><span class="sxs-lookup"><span data-stu-id="71b41-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="71b41-105">Mẫu</span><span class="sxs-lookup"><span data-stu-id="71b41-105">Example:</span></span>

<span data-ttu-id="71b41-106">Người dùng Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="71b41-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="71b41-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="71b41-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="71b41-108">Hãy chờ ít nhất một giờ để thay đổi có hiệu lực.</span><span class="sxs-lookup"><span data-stu-id="71b41-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="71b41-109">Nếu vẫn là vấn đề, vui lòng làm theo [quy trình này](https://aka.ms/pfcte) để khắc phục sự cố truy nhập thư mục công cộng bằng cách dùng Outlook.</span><span class="sxs-lookup"><span data-stu-id="71b41-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="71b41-110">**Để điều khiển người dùng có thể truy nhập vào các thư mục công cộng bằng cách dùng Outlook**:</span><span class="sxs-lookup"><span data-stu-id="71b41-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="71b41-111">Sử dụng Set-CASMailbox <mailboxname> -publicfolderaccess $True hoặc $false</span><span class="sxs-lookup"><span data-stu-id="71b41-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="71b41-112">$true: cho phép người dùng truy nhập các thư mục công cộng trong Outlook</span><span class="sxs-lookup"><span data-stu-id="71b41-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="71b41-113">$false: ngăn chặn quyền truy nhập của người dùng vào các thư mục công cộng trong Outlook.</span><span class="sxs-lookup"><span data-stu-id="71b41-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="71b41-114">Đây là giá trị mặc định.</span><span class="sxs-lookup"><span data-stu-id="71b41-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="71b41-115">Các $true Set-OrganizationConfig-Publicfolderđiều khiển</span><span class="sxs-lookup"><span data-stu-id="71b41-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="71b41-116">**Ghi chú** Quy trình này chỉ có thể kiểm soát các kết nối với Outlook trên máy tính cho máy khách chạy Windows.</span><span class="sxs-lookup"><span data-stu-id="71b41-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="71b41-117">Người dùng có thể tiếp tục truy nhập vào các thư mục công cộng bằng OWA hoặc Outlook for Mac.</span><span class="sxs-lookup"><span data-stu-id="71b41-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="71b41-118">Để biết thêm thông tin, hãy xem thông [báo hỗ trợ các kết nối được kiểm soát đến các thư mục công cộng trong Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="71b41-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>