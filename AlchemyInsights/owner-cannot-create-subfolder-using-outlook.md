---
title: Chủ sở hữu không thể tạo thư mục con bằng cách sử dụng Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749237"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="91f90-102">Chủ sở hữu không thể tạo thư mục con bằng cách sử dụng Outlook</span><span class="sxs-lookup"><span data-stu-id="91f90-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="91f90-103">**Có một vấn đề đang diễn ra với chủ sở hữu thư mục công cộng tạo các cặp con sử dụng Outlook. Vấn đề sẽ được cố định sớm.**</span><span class="sxs-lookup"><span data-stu-id="91f90-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="91f90-104">Trong khi đó, sử dụng một trong các giải pháp sau:</span><span class="sxs-lookup"><span data-stu-id="91f90-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="91f90-105">Sử dụng Outlook dành cho MAC để tạo thư mục con khi sự cố ảnh hưởng đến chỉ Outlook cho máy tính để bàn Windows (Tất cả các phiên bản)</span><span class="sxs-lookup"><span data-stu-id="91f90-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="91f90-106">Có quản trị viên tạo thư mục con bằng cách sử dụng EXO Shell hoặc EAC</span><span class="sxs-lookup"><span data-stu-id="91f90-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="91f90-107">Thay đổi DefaultPublicFolderMailbox/EffectivePublicFolderMailbox trên người dùng hộp thư khác với hộp thư nội dung cho thư mục gây ra sự cố</span><span class="sxs-lookup"><span data-stu-id="91f90-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="91f90-108">*Thiết lập hộp thư 1 đã DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="91f90-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="91f90-109">Đợi một giờ, khởi động lại máy khách Outlook</span><span class="sxs-lookup"><span data-stu-id="91f90-109">Wait for an hour, restart outlook client</span></span>