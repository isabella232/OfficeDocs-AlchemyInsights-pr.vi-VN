---
title: Thay đổi địa chỉ email của nhóm Microsoft 365
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
- "1200024"
- "4704"
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48462062"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="57a81-102">Thay đổi địa chỉ email của một nhóm Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="57a81-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="57a81-103">Bạn có thể thay đổi địa chỉ email của một nhóm Microsoft 365 bằng cách sử dụng trung tâm quản trị.</span><span class="sxs-lookup"><span data-stu-id="57a81-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="57a81-104">Chỉ cần chọn Nhóm và chọn @edit địa chỉ email.</span><span class="sxs-lookup"><span data-stu-id="57a81-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="57a81-105">Bạn cũng có thể sử dụng theo dõi lệnh EXO PowerShell để thay đổi địa chỉ SMTP chính của nhóm Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="57a81-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="57a81-106">Mẫu</span><span class="sxs-lookup"><span data-stu-id="57a81-106">Example:</span></span>

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
