---
title: Chủ sở hữu không thể tạo thư mục con bằng cách dùng Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665740"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="62057-102">Chủ sở hữu không thể tạo thư mục con bằng cách dùng Outlook</span><span class="sxs-lookup"><span data-stu-id="62057-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="62057-103">**Có vấn đề liên tiếp với chủ sở hữu thư mục công cộng tạo thư mục con bằng cách dùng Outlook. Vấn đề sẽ sớm được khắc phục.**</span><span class="sxs-lookup"><span data-stu-id="62057-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="62057-104">Trong khi đó, hãy dùng một trong các giải pháp thay thế sau đây:</span><span class="sxs-lookup"><span data-stu-id="62057-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="62057-105">Sử dụng Outlook for MAC để tạo thư mục con là sự cố chỉ tác động đến Windows for Desktop (Tất cả các phiên bản)</span><span class="sxs-lookup"><span data-stu-id="62057-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="62057-106">Quản trị tạo thư mục con bằng EXO Shell hoặc EAC</span><span class="sxs-lookup"><span data-stu-id="62057-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="62057-107">Thay đổi DefaultPublicFolderMailbox/EffectivePublicFolderMailbox trên người dùng đến hộp thư khác ngoài hộp thư nội dung cho thư mục gây ra sự cố</span><span class="sxs-lookup"><span data-stu-id="62057-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="62057-108">*Set-Mailbox user1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="62057-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="62057-109">Chờ một giờ, khởi động lại ứng dụng khách Outlook</span><span class="sxs-lookup"><span data-stu-id="62057-109">Wait for an hour, restart outlook client</span></span>