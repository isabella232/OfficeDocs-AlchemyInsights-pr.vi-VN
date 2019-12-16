---
title: Không thể xoá các mục trong SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049539"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="4e1ee-102">Không thể xoá các mục</span><span class="sxs-lookup"><span data-stu-id="4e1ee-102">Unable to delete items</span></span>

<span data-ttu-id="4e1ee-103">Có vấn đề xóa các mục SharePoint?</span><span class="sxs-lookup"><span data-stu-id="4e1ee-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="4e1ee-104">Luôn đảm bảo rằng bạn có quyền [thích hợp](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) để xoá mục hoặc có một [quản trị viên bộ sưu tập trang web](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) cố gắng loại bỏ mục.</span><span class="sxs-lookup"><span data-stu-id="4e1ee-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="4e1ee-105">Đảm bảo rằng không có thiết lập [chính sách lưu giữ](https://docs.microsoft.com/office365/securitycompliance/retention-policies) trên mục.</span><span class="sxs-lookup"><span data-stu-id="4e1ee-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="4e1ee-106">Đảm bảo mục không được [kiểm tra](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) cho người dùng khác.</span><span class="sxs-lookup"><span data-stu-id="4e1ee-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="4e1ee-107">Cuối cùng, quản trị viên có thể sử dụng [SharePoint Patterns và thực tiễn](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) chứa một thư viện lệnh PowerShell cho phép bạn thực hiện các hành động quản lý phức tạp như lực xóa các mục cứng đầu.</span><span class="sxs-lookup"><span data-stu-id="4e1ee-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="4e1ee-108">Loại bỏ PNP file</span><span class="sxs-lookup"><span data-stu-id="4e1ee-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="4e1ee-109">Loại bỏ PNP cặp</span><span class="sxs-lookup"><span data-stu-id="4e1ee-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="4e1ee-110">Loại bỏ PNP danh mục</span><span class="sxs-lookup"><span data-stu-id="4e1ee-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="4e1ee-111">Loại bỏ PNP danh sách</span><span class="sxs-lookup"><span data-stu-id="4e1ee-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="4e1ee-112">Loại bỏ PNP trường (cột)</span><span class="sxs-lookup"><span data-stu-id="4e1ee-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)