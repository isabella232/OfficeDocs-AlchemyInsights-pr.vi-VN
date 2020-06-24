---
title: Quyền lịch
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862162"
---
# <a name="calendar-permissions"></a><span data-ttu-id="112b4-102">Quyền lịch</span><span class="sxs-lookup"><span data-stu-id="112b4-102">Calendar Permissions</span></span>

<span data-ttu-id="112b4-103">Người dùng có thể thay đổi quyền lịch của riêng mình với Outlook trên web hoặc các máy khách khác, nhưng là quản trị viên mà bạn có thể cần điều tra là tốt.</span><span class="sxs-lookup"><span data-stu-id="112b4-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="112b4-104">Với lệnh ghép ngắn Exchange PowerShell sẽ hiển thị cho bạn quyền trên lịch của người dùng:</span><span class="sxs-lookup"><span data-stu-id="112b4-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="112b4-105">Để xem thêm thông tin, hãy xem mục sau:</span><span class="sxs-lookup"><span data-stu-id="112b4-105">To see more information see the following:</span></span>

- [<span data-ttu-id="112b4-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="112b4-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="112b4-107">Thiết lập MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="112b4-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="112b4-108">Thêm MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="112b4-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="112b4-109">Quyền lịch được sử dụng trong việc chia sẻ lịch, để xem thêm thông tin về chia sẻ lịch Outlook, hãy xem các bài viết này:</span><span class="sxs-lookup"><span data-stu-id="112b4-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="112b4-110">Chia sẻ lịch Outlook với người khác</span><span class="sxs-lookup"><span data-stu-id="112b4-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="112b4-111">Chia sẻ lịch của bạn trong Outlook trên web cho doanh nghiệp</span><span class="sxs-lookup"><span data-stu-id="112b4-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="112b4-112">Để khắc phục sự cho phép lịch bạn có thể sử dụng công cụ [hỗ trợ và trợ lý phục hồi](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .</span><span class="sxs-lookup"><span data-stu-id="112b4-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>