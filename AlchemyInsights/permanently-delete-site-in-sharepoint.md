---
title: Xóa vĩnh viễn một site trong SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: bde31f9b197118467ed96d665a9c8edf6b789965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771743"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="29fb5-102">Xóa vĩnh viễn một site trong SharePoint</span><span class="sxs-lookup"><span data-stu-id="29fb5-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="29fb5-103">Để sử dụng lại một URL từ một site đã xóa (để tạo lại một site), hoặc để xóa vĩnh viễn một site vì không còn sử dụng được nữa, bạn có thể dùng **xóa vĩnh viễn** khỏi Trung tâm quản trị SharePoint mới.</span><span class="sxs-lookup"><span data-stu-id="29fb5-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="29fb5-104">Đi đến [trang site đã xóa của Trung tâm quản trị SharePoint mới](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) và đăng nhập bằng tài khoản có quyền quản trị cho tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="29fb5-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="29fb5-105">Trong cột bên trái, hãy chọn một site.</span><span class="sxs-lookup"><span data-stu-id="29fb5-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="29fb5-106">Bấm **xóa vĩnh viễn**.</span><span class="sxs-lookup"><span data-stu-id="29fb5-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="29fb5-107">**Lưu ý**: các site kết nối nhóm không thể bị xóa vĩnh viễn khỏi Trung tâm quản trị SharePoint mới.</span><span class="sxs-lookup"><span data-stu-id="29fb5-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="29fb5-108">[Loại bỏ-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) sẽ cần được sử dụng thay vào đó.</span><span class="sxs-lookup"><span data-stu-id="29fb5-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="29fb5-109">Để biết thêm thông tin, hãy xem mục [xóa vĩnh viễn một site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="29fb5-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
