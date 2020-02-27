---
title: Tạo một email bắt tất cả
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286313"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="6f969-102">Tạo một email bắt tất cả</span><span class="sxs-lookup"><span data-stu-id="6f969-102">Create an email catch all</span></span>

<span data-ttu-id="6f969-103">Sử dụng một nắm bắt tất cả được khuyến khích mạnh mẽ.</span><span class="sxs-lookup"><span data-stu-id="6f969-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="6f969-104">Nó là tốt hơn để cung cấp một thư bị trả lại cho người gửi cho phép gửi biết tin nhắn của họ không thể được gửi như là địa chỉ để họ có thể thực hiện hành động.</span><span class="sxs-lookup"><span data-stu-id="6f969-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="6f969-105">Bạn cũng có thể hạn chế hộp thư theo dõi để chỉ bắt trước đây địa chỉ email hợp lệ.</span><span class="sxs-lookup"><span data-stu-id="6f969-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="6f969-106">Bất kỳ bắt tất cả các hộp thư sẽ nhận được một thỏa thuận tốt của thư rác và cuối cùng có thể điền nếu không theo dõi chặt chẽ.</span><span class="sxs-lookup"><span data-stu-id="6f969-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="6f969-107">(Có những giới hạn nhận được.)</span><span class="sxs-lookup"><span data-stu-id="6f969-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="6f969-108">Nếu bạn quyết định tiếp tục, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="6f969-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="6f969-109">Tạo nhóm phân phối động & bao gồm "tất cả các loại người nhận."</span><span class="sxs-lookup"><span data-stu-id="6f969-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="6f969-110">Tạo một hộp thư chuyên dụng để bắt email, ví dụ: catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="6f969-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="6f969-111">Đối với miền cụ thể, đặt DomainType "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="6f969-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="6f969-112">Nếu sau đó bạn loại bỏ tất cả các bắt, hãy chắc chắn để đặt tên miền trở lại uỷ quyền.</span><span class="sxs-lookup"><span data-stu-id="6f969-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="6f969-113">Tạo quy tắc truyền tải Mailflow như sau:</span><span class="sxs-lookup"><span data-stu-id="6f969-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="6f969-114">Nếu người gửi là "bên ngoài tổ chức"</span><span class="sxs-lookup"><span data-stu-id="6f969-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="6f969-115">Chuyển hướng thư đến Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="6f969-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="6f969-116">Ngoại trừ nếu người nhận là thành viên của allusers@domain.com (nhóm phân phối chứa tất cả các thành viên)</span><span class="sxs-lookup"><span data-stu-id="6f969-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="6f969-117">Đảm bảo xác nhận rằng hộp thư mới được thêm vào nhóm phân phối động</span><span class="sxs-lookup"><span data-stu-id="6f969-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
