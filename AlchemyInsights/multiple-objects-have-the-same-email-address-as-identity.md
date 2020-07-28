---
title: Nhiều đối tượng có cùng địa chỉ email như danh tính
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439705"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="0bb34-102">Nhiều đối tượng có cùng địa chỉ email như danh tính</span><span class="sxs-lookup"><span data-stu-id="0bb34-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="0bb34-103">**Nhiều đối tượng**</span><span class="sxs-lookup"><span data-stu-id="0bb34-103">**Multiple objects**</span></span>

<span data-ttu-id="0bb34-104">Một trong những lý do phổ biến của lỗi này không thể định tuyến một yêu cầu Outlook Web Access đúng trong sự hiện diện của nhiều đối tượng có cùng địa chỉ email như danh tính.</span><span class="sxs-lookup"><span data-stu-id="0bb34-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="0bb34-105">Để tìm các đối tượng này, hãy chạy lệnh sau:</span><span class="sxs-lookup"><span data-stu-id="0bb34-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="0bb34-106">· Nhận-người nhận<email address></span><span class="sxs-lookup"><span data-stu-id="0bb34-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="0bb34-107">· Get-người dùng<email address></span><span class="sxs-lookup"><span data-stu-id="0bb34-107">· Get-User <email address></span></span>

<span data-ttu-id="0bb34-108">· Nhận-người dùng <email address> -softdeleteduser</span><span class="sxs-lookup"><span data-stu-id="0bb34-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="0bb34-109">· Get-liên hệ<email address></span><span class="sxs-lookup"><span data-stu-id="0bb34-109">· Get-Contact <email address></span></span>

<span data-ttu-id="0bb34-110">· Nhận hộp thư <email address> -publicfolder</span><span class="sxs-lookup"><span data-stu-id="0bb34-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="0bb34-111">· Nhận hộp thư <email address> -includesoftdeletedmailbox</span><span class="sxs-lookup"><span data-stu-id="0bb34-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="0bb34-112">· Nhận được-Mailbox <email address> -inactivemailboxonly</span><span class="sxs-lookup"><span data-stu-id="0bb34-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="0bb34-113">Để khắc phục sự cố, loại bỏ nhiều đối tượng với nhận dạng email cùng và đảm bảo rằng có một đối tượng duy nhất với danh tính email cụ thể và loại người nhận là UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="0bb34-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="0bb34-114">**Cùng một địa chỉ được sử dụng cho doanh nghiệp và người tiêu dùng hộp thư**</span><span class="sxs-lookup"><span data-stu-id="0bb34-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="0bb34-115">Nguyên nhân khác là khi cùng một địa chỉ được sử dụng cho doanh nghiệp và người tiêu dùng hộp thư.</span><span class="sxs-lookup"><span data-stu-id="0bb34-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="0bb34-116">Trong trường hợp này, người dùng phải thay đổi bí danh tiêu dùng chính của họ cho đến khi Cafe hỗ trợ kịch bản này.</span><span class="sxs-lookup"><span data-stu-id="0bb34-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="0bb34-117">Đây là một lỗi vĩnh viễn mà không đi xa mà không can thiệp.</span><span class="sxs-lookup"><span data-stu-id="0bb34-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="0bb34-118">Để biết chi tiết, hãy xem [thay đổi địa chỉ email hoặc số điện thoại cho tài khoản Microsoft của bạn](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="0bb34-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>