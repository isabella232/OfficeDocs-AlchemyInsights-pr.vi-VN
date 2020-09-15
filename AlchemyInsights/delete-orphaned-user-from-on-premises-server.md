---
title: Xóa người dùng mồ côi từ máy chủ tại cơ sở
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680157"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="3f93a-102">Xóa người dùng mồ côi từ máy chủ tại cơ sở</span><span class="sxs-lookup"><span data-stu-id="3f93a-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="3f93a-103">Để loại bỏ một người dùng mồ côi, hãy làm theo các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="3f93a-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="3f93a-104">Đồng bộ hóa Directory bằng cách làm theo các hướng dẫn trong [danh tính hỗn hợp với Azure Active Directory là gì?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="3f93a-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="3f93a-105">Để xác minh việc đồng bộ hóa thư mục, hãy xem [danh tính kết hợp với Azure Active Directory là gì?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="3f93a-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="3f93a-106">Nếu các hàm đồng bộ chính xác nhưng việc xóa đối tượng Active Directory không được tuyên truyền với Azure AD, hãy loại bỏ các đối tượng mồ côi bằng cách dùng một trong các lệnh ghép ngắn Azure Active Directory cho Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="3f93a-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="3f93a-107">Loại bỏ-MsolContact</span><span class="sxs-lookup"><span data-stu-id="3f93a-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="3f93a-108">Loại bỏ-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="3f93a-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="3f93a-109">Loại bỏ-MsolUser</span><span class="sxs-lookup"><span data-stu-id="3f93a-109">Remove-MsolUser</span></span>

    <span data-ttu-id="3f93a-110">Ví dụ: để loại bỏ người dùng mồ côi ID john.smith@contoso.com, ban đầu được tạo bằng cách sử dụng đồng bộ hóa thư mục, hãy chạy lệnh ghép ngắn:</span><span class="sxs-lookup"><span data-stu-id="3f93a-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="3f93a-111">Loại bỏ-MsolUser – UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="3f93a-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>