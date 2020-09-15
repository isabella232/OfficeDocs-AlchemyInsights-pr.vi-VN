---
title: Tạo một email bắt tất cả
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713008"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="bff3f-102">Tạo một email bắt tất cả</span><span class="sxs-lookup"><span data-stu-id="bff3f-102">Create an email catch all</span></span>

<span data-ttu-id="bff3f-103">Sử dụng tất cả bắt được khuyến khích mạnh mẽ.</span><span class="sxs-lookup"><span data-stu-id="bff3f-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="bff3f-104">Tốt hơn là nên cung cấp một bản phân phát trở lại người gửi cho phép người gửi biết thư của họ không thể chuyển phát như địa chỉ để họ có thể thực hiện hành động.</span><span class="sxs-lookup"><span data-stu-id="bff3f-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="bff3f-105">Bạn cũng có thể giới hạn hộp thư theo dõi để chỉ bắt đầu trước đây là địa chỉ email hợp lệ.</span><span class="sxs-lookup"><span data-stu-id="bff3f-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="bff3f-106">Bất kỳ hộp thư nào nắm bắt tất cả sẽ nhận được nhiều thư rác và cuối cùng có thể điền vào nếu không được giám sát chặt chẽ.</span><span class="sxs-lookup"><span data-stu-id="bff3f-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="bff3f-107">(Có các giới hạn tiếp nhận.)</span><span class="sxs-lookup"><span data-stu-id="bff3f-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="bff3f-108">Nếu bạn quyết định tiếp tục, hãy làm theo các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="bff3f-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="bff3f-109">Tạo một nhóm phân phối động & bao gồm "tất cả các loại người nhận."</span><span class="sxs-lookup"><span data-stu-id="bff3f-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="bff3f-110">Tạo hộp thư chuyên biệt để bắt email, ví dụ, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="bff3f-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="bff3f-111">Đối với tên miền cụ thể, hãy đặt kiểu DomainType thành "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="bff3f-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="bff3f-112">Nếu sau đó bạn loại bỏ tất cả bắt kịp, hãy đảm bảo đặt tên miền trở lại thẩm quyền.</span><span class="sxs-lookup"><span data-stu-id="bff3f-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="bff3f-113">Tạo một quy tắc truyền dẫn dòng thư như sau:</span><span class="sxs-lookup"><span data-stu-id="bff3f-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="bff3f-114">Nếu người gửi là "bên ngoài tổ chức"</span><span class="sxs-lookup"><span data-stu-id="bff3f-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="bff3f-115">Chuyển hướng thư đến Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="bff3f-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="bff3f-116">Trừ khi người nhận là thành viên của allusers@domain.com (nhóm phân phối chứa tất cả thành viên)</span><span class="sxs-lookup"><span data-stu-id="bff3f-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="bff3f-117">Đảm bảo xác thực rằng các hộp thư mới được thêm vào nhóm phân phối động</span><span class="sxs-lookup"><span data-stu-id="bff3f-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
