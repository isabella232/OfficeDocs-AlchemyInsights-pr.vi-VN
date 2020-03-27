---
title: Xóa vĩnh viễn một trang web trong SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955231"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="556ac-102">Xóa vĩnh viễn một trang web trong SharePoint</span><span class="sxs-lookup"><span data-stu-id="556ac-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="556ac-103">Để tái sử dụng URL từ một trang web đã xóa (để tạo lại một trang web) hoặc xóa vĩnh viễn một trang web vì nó không còn dùng nữa, bạn có thể sử dụng **xóa vĩnh viễn** khỏi Trung tâm quản trị SharePoint mới.</span><span class="sxs-lookup"><span data-stu-id="556ac-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="556ac-104">Đi tới [trang trang web đã xóa của Trung tâm quản trị SharePoint mới](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) và đăng nhập bằng tài khoản có quyền quản trị cho tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="556ac-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="556ac-105">Trong cột bên trái, chọn một trang web.</span><span class="sxs-lookup"><span data-stu-id="556ac-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="556ac-106">Nhấp vào **xóa vĩnh viễn**.</span><span class="sxs-lookup"><span data-stu-id="556ac-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="556ac-107">**Lưu ý**: không thể xóa vĩnh viễn các trang web được kết nối với nhóm khỏi Trung tâm quản trị SharePoint mới.</span><span class="sxs-lookup"><span data-stu-id="556ac-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="556ac-108">[Loại bỏ-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) sẽ cần phải được sử dụng để thay thế.</span><span class="sxs-lookup"><span data-stu-id="556ac-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="556ac-109">Để biết thêm thông tin, xem [xóa vĩnh viễn trang web](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="556ac-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
