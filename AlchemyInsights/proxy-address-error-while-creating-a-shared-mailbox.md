---
title: Lỗi địa chỉ proxy trong khi tạo hộp thư dùng chung
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568312"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="80257-102">Lỗi địa chỉ proxy trong khi tạo một hộp thư hoặc đối tượng được kích hoạt email khác</span><span class="sxs-lookup"><span data-stu-id="80257-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="80257-103">Nếu bạn đã tìm cách tạo đối tượng cho phép email (hộp thư, hộp thư chung, v.v.) và nhận được lỗi "địa chỉ proxy" SMTP:alias@domain.com "đang được sử dụng...", địa chỉ email mà bạn đã chọn đã được thực hiện bởi một đối tượng được kích hoạt email khác trong tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="80257-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="80257-104">Bạn cần tìm kiếm người dùng, nhóm, hộp thư chung hoặc thư mục công cộng có địa chỉ email này và xóa nó hoặc thay đổi địa chỉ email của nó.</span><span class="sxs-lookup"><span data-stu-id="80257-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="80257-105">Sau đó, bạn có thể tạo đối tượng có hỗ trợ email mới với địa chỉ email được giải phóng.</span><span class="sxs-lookup"><span data-stu-id="80257-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="80257-106">Sử dụng tìm kiếm trên trang chủ để tìm nó.</span><span class="sxs-lookup"><span data-stu-id="80257-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="80257-107">Bạn cũng có thể sử dụng lệnh Exchange Online PowerShell sau đây để tìm kiếm:</span><span class="sxs-lookup"><span data-stu-id="80257-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="80257-108">Nếu bạn không muốn xóa địa chỉ email hiện có, hãy chọn một địa chỉ email mới cho đối tượng mới mà bạn đang tạo.</span><span class="sxs-lookup"><span data-stu-id="80257-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  