---
title: Thay đổi địa chỉ email của một nhóm Microsoft 365 hoặc Microsoft nhóm
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819102"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="85908-102">Thay đổi địa chỉ email của một nhóm Microsoft 365 hoặc Microsoft nhóm</span><span class="sxs-lookup"><span data-stu-id="85908-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="85908-103">Bạn có thể thay đổi địa chỉ email của một nhóm Microsoft 365 hoặc các nhóm Microsoft bằng cách sử dụng [Trung tâm quản trị microsoft 365](https://admin.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="85908-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="85908-104">Chỉ cần chọn Nhóm và chọn @edit địa chỉ email.</span><span class="sxs-lookup"><span data-stu-id="85908-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="85908-105">Bạn cũng có thể sử dụng lệnh EXO PowerShell sau đây để thay đổi địa chỉ SMTP chính của một nhóm Microsoft 365/Nhóm:</span><span class="sxs-lookup"><span data-stu-id="85908-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="85908-106">Mẫu</span><span class="sxs-lookup"><span data-stu-id="85908-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
