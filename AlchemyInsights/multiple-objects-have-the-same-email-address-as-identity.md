---
title: Nhiều đối tượng có cùng địa chỉ email với danh tính
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724637"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="64c60-102">Nhiều đối tượng có cùng địa chỉ email với danh tính</span><span class="sxs-lookup"><span data-stu-id="64c60-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="64c60-103">**Nhiều đối tượng**</span><span class="sxs-lookup"><span data-stu-id="64c60-103">**Multiple objects**</span></span>

<span data-ttu-id="64c60-104">Một trong những lý do phổ biến của lỗi này không thể định tuyến một yêu cầu Outlook Web Access đúng cách với sự hiện diện của nhiều đối tượng có cùng địa chỉ email với danh tính.</span><span class="sxs-lookup"><span data-stu-id="64c60-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="64c60-105">Để tìm các đối tượng này, hãy chạy các lệnh sau đây:</span><span class="sxs-lookup"><span data-stu-id="64c60-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="64c60-106">· Get-người nhận <email address></span><span class="sxs-lookup"><span data-stu-id="64c60-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="64c60-107">· Get-User <email address></span><span class="sxs-lookup"><span data-stu-id="64c60-107">· Get-User <email address></span></span>

<span data-ttu-id="64c60-108">· Get-User <email address> -softdeleteduser</span><span class="sxs-lookup"><span data-stu-id="64c60-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="64c60-109">· Get-liên hệ <email address></span><span class="sxs-lookup"><span data-stu-id="64c60-109">· Get-Contact <email address></span></span>

<span data-ttu-id="64c60-110">· Tải thư mục được đăng ký hộp thư <email address></span><span class="sxs-lookup"><span data-stu-id="64c60-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="64c60-111">· Get-hộp thư <email address> -includesoftdeletedmailbox</span><span class="sxs-lookup"><span data-stu-id="64c60-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="64c60-112">· Get-Mailbox <email address> -inactivemailboxonly</span><span class="sxs-lookup"><span data-stu-id="64c60-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="64c60-113">Để giải quyết vấn đề này, hãy loại bỏ nhiều đối tượng với cùng một danh tính email và đảm bảo rằng có một đối tượng duy nhất với danh tính email cụ thể và loại người nhận đó là hộp thư user.</span><span class="sxs-lookup"><span data-stu-id="64c60-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="64c60-114">**Cùng một địa chỉ được sử dụng cho các hộp thư kinh doanh và người tiêu dùng**</span><span class="sxs-lookup"><span data-stu-id="64c60-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="64c60-115">Nguyên nhân khác là khi cùng một địa chỉ được sử dụng cho các hộp thư kinh doanh và người dùng.</span><span class="sxs-lookup"><span data-stu-id="64c60-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="64c60-116">Trong trường hợp này, người dùng phải thay đổi biệt danh người tiêu dùng chính của họ cho đến khi Cafe hỗ trợ kịch bản này.</span><span class="sxs-lookup"><span data-stu-id="64c60-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="64c60-117">Đây là lỗi cố định không biến mất nếu không có can thiệp.</span><span class="sxs-lookup"><span data-stu-id="64c60-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="64c60-118">Để biết chi tiết, hãy xem [thay đổi địa chỉ email hoặc số điện thoại cho tài khoản Microsoft của bạn](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="64c60-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>