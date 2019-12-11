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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959516"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="05ce9-102">Outlook không thể kết nối với thư mục công cộng</span><span class="sxs-lookup"><span data-stu-id="05ce9-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="05ce9-103">Nếu truy cập thư mục công cộng không hoạt động cho một số người dùng, hãy thử như sau:</span><span class="sxs-lookup"><span data-stu-id="05ce9-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="05ce9-104">Kết nối với EXO PowerShell và đặt cấu hình DefaultPublicFolderMailbox trên tài khoản người dùng sự cố để phù hợp với một tài khoản người dùng đang hoạt động.</span><span class="sxs-lookup"><span data-stu-id="05ce9-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="05ce9-105">Ví dụ:</span><span class="sxs-lookup"><span data-stu-id="05ce9-105">Example:</span></span>

<span data-ttu-id="05ce9-106">Get-Mailbox Workingngười dùng | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="05ce9-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="05ce9-107">Set-hộp thư ProblemUser-DefaultPublicFolderMailbox \<giá trị từ lệnh trước></span><span class="sxs-lookup"><span data-stu-id="05ce9-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="05ce9-108">Hãy đợi ít nhất một giờ để thay đổi có hiệu lực.</span><span class="sxs-lookup"><span data-stu-id="05ce9-108">Wait at least one hour for the change to take effect.</span></span>