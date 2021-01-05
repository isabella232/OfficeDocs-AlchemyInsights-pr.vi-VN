---
title: Thay đổi địa chỉ email của một nhóm Microsoft 365 hoặc Microsoft nhóm
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756579"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="1713d-102">Thay đổi địa chỉ email của một nhóm Microsoft 365 hoặc Microsoft nhóm</span><span class="sxs-lookup"><span data-stu-id="1713d-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="1713d-103">Bạn có thể thay đổi địa chỉ email của một nhóm Microsoft 365 hoặc các nhóm Microsoft bằng cách sử dụng [Trung tâm quản trị microsoft 365](https://admin.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="1713d-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="1713d-104">Chỉ cần chọn Nhóm và chọn @edit địa chỉ email.</span><span class="sxs-lookup"><span data-stu-id="1713d-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="1713d-105">Bạn cũng có thể sử dụng lệnh EXO PowerShell sau đây để thay đổi địa chỉ SMTP chính của một nhóm Microsoft 365/Nhóm:</span><span class="sxs-lookup"><span data-stu-id="1713d-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="1713d-106">Mẫu</span><span class="sxs-lookup"><span data-stu-id="1713d-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
