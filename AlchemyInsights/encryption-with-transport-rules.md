---
title: Mã hóa với quy tắc truyền dẫn
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
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813890"
---
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="35ed4-102">Mã hóa với quy tắc truyền dẫn</span><span class="sxs-lookup"><span data-stu-id="35ed4-102">Encryption with transport rules</span></span>

<span data-ttu-id="35ed4-103">Trong [Trung tâm quản trị Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), bạn có thể sử dụng các chức năng mã hóa tin nhắn Office (OME) trong các quy tắc dòng thư để kích hoạt mã hóa thư.</span><span class="sxs-lookup"><span data-stu-id="35ed4-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="35ed4-104">Chọn tùy chọn **áp dụng mã hóa thư Office 365 và bảo vệ quyền** trên điều kiện quy tắc truyền dẫn.</span><span class="sxs-lookup"><span data-stu-id="35ed4-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="35ed4-105">Để biết thêm thông tin, hãy xem mục [xác định quy tắc dòng thư để mã hóa](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="35ed4-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="35ed4-106">Trong PowerShell, sử dụng lệnh ghép ngắn [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) và đặt tham số *applyome* sang $True.</span><span class="sxs-lookup"><span data-stu-id="35ed4-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>
