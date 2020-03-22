---
title: Không thể truy cập thư mục công cộng
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891771"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="d2a24-102">Outlook không thể kết nối với thư mục công cộng</span><span class="sxs-lookup"><span data-stu-id="d2a24-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="d2a24-103">Nếu truy cập thư mục công cộng không hoạt động đối với một số người dùng, hãy thử như sau:</span><span class="sxs-lookup"><span data-stu-id="d2a24-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="d2a24-104">Kết nối với EXO PowerShell và đặt cấu hình tham số DefaultPublicFolderMailbox trên tài khoản người dùng sự cố để phù hợp với tham số trên tài khoản người dùng đang hoạt động.</span><span class="sxs-lookup"><span data-stu-id="d2a24-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="d2a24-105">Ví dụ:</span><span class="sxs-lookup"><span data-stu-id="d2a24-105">Example:</span></span>

<span data-ttu-id="d2a24-106">Get-Mailbox Workingngười dùng | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="d2a24-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="d2a24-107">Set-hộp thư ProblemUser-DefaultPublicFolderMailbox \<giá trị từ lệnh trước></span><span class="sxs-lookup"><span data-stu-id="d2a24-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="d2a24-108">Hãy đợi ít nhất một giờ để thay đổi có hiệu lực.</span><span class="sxs-lookup"><span data-stu-id="d2a24-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="d2a24-109">Nếu sự cố vẫn còn, hãy làm theo [quy trình này](https://aka.ms/pfcte) để khắc phục sự cố truy cập thư mục công cộng bằng cách sử dụng Outlook.</span><span class="sxs-lookup"><span data-stu-id="d2a24-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>