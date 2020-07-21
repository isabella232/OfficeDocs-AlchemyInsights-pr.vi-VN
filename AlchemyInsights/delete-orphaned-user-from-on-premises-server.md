---
title: Xoá người dùng đơn lẻ từ máy chủ tại chỗ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198582"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="c3068-102">Xoá người dùng đơn lẻ từ máy chủ tại chỗ</span><span class="sxs-lookup"><span data-stu-id="c3068-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="c3068-103">Để loại bỏ người dùng đơn lẻ, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="c3068-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="c3068-104">Áp dụng đồng bộ hóa thư mục bằng cách làm theo hướng dẫn trong [danh tính lai với Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="c3068-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="c3068-105">Để xác minh đồng bộ hóa thư mục, xem [danh tính lai với Azure Active Directory là gì?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="c3068-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="c3068-106">Nếu đồng bộ hoá chức năng chính xác nhưng xoá đối tượng Active Directory không tuyên truyền Azure AD, xoá thủ công các đối tượng đơn lẻ bằng cách sử dụng một trong các lệnh ghép ngắn Azure Active Directory mô-đun Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="c3068-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="c3068-107">Loại bỏ-MsolContact</span><span class="sxs-lookup"><span data-stu-id="c3068-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="c3068-108">Loại bỏ-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="c3068-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="c3068-109">Loại bỏ-MsolUser</span><span class="sxs-lookup"><span data-stu-id="c3068-109">Remove-MsolUser</span></span>

    <span data-ttu-id="c3068-110">Ví dụ: để loại bỏ người dùng đơn lẻ ID john.smith@contoso.com, ban đầu được tạo ra bằng cách sử dụng đồng bộ hóa thư mục, chạy lệnh:</span><span class="sxs-lookup"><span data-stu-id="c3068-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="c3068-111">Loại bỏ-MsolUser-UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="c3068-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>