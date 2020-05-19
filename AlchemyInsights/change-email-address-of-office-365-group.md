---
title: Thay đổi địa chỉ email của một nhóm Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/27/2020
ms.locfileid: "44283266"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="8a02a-102">Thay đổi địa chỉ email của một nhóm Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="8a02a-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="8a02a-103">Bạn có thể thay đổi địa chỉ email của một nhóm Microsoft 365 bằng cách sử dụng trung tâm quản trị.</span><span class="sxs-lookup"><span data-stu-id="8a02a-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="8a02a-104">Chỉ cần chọn Nhóm và chọn @edit địa chỉ email.</span><span class="sxs-lookup"><span data-stu-id="8a02a-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="8a02a-105">Bạn cũng có thể sử dụng sau lệnh EXO PowerShell để thay đổi địa chỉ SMTP chính của một nhóm Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="8a02a-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="8a02a-106">Thiết lập UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="8a02a-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="8a02a-107">Ví dụ:</span><span class="sxs-lookup"><span data-stu-id="8a02a-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
