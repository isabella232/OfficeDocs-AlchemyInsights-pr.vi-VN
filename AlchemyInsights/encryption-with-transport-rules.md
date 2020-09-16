---
title: Mã hóa với quy tắc truyền dẫn
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
- "9002635"
- "5154"
ms.openlocfilehash: 4c43fc16db84832c4e2aa3b6483632de6861b877
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784365"
---
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="8ef7e-102">Mã hóa với quy tắc truyền dẫn</span><span class="sxs-lookup"><span data-stu-id="8ef7e-102">Encryption with transport rules</span></span>

<span data-ttu-id="8ef7e-103">Trong [Trung tâm quản trị Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), bạn có thể sử dụng các chức năng mã hóa tin nhắn Office (OME) trong các quy tắc dòng thư để kích hoạt mã hóa thư.</span><span class="sxs-lookup"><span data-stu-id="8ef7e-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="8ef7e-104">Chọn tùy chọn **áp dụng mã hóa thư Office 365 và bảo vệ quyền** trên điều kiện quy tắc truyền dẫn.</span><span class="sxs-lookup"><span data-stu-id="8ef7e-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="8ef7e-105">Để biết thêm thông tin, hãy xem mục [xác định quy tắc dòng thư để mã hóa](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="8ef7e-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="8ef7e-106">Trong PowerShell, sử dụng lệnh ghép ngắn [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) và đặt tham số *applyome* sang $True.</span><span class="sxs-lookup"><span data-stu-id="8ef7e-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>
