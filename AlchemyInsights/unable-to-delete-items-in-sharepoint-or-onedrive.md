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
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571293"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="6275e-102">Không thể xoá các mục</span><span class="sxs-lookup"><span data-stu-id="6275e-102">Unable to delete items</span></span>

<span data-ttu-id="6275e-103">Chính sách lưu giữ có thể gây ra điều này, bạn cần tắt hoặc loại trừ các giữ tương ứng gây ra vấn đề này.</span><span class="sxs-lookup"><span data-stu-id="6275e-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="6275e-104">Sau khi chính sách lưu giữ hoặc giữ bị xóa, có thể mất đến 24 giờ để thay đổi có hiệu lực.</span><span class="sxs-lookup"><span data-stu-id="6275e-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="6275e-105">Đảm bảo rằng không có thiết lập [chính sách lưu giữ](https://docs.microsoft.com/office365/securitycompliance/retention-policies) trên mục.</span><span class="sxs-lookup"><span data-stu-id="6275e-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="6275e-106">Trang web có thể vượt quá giới hạn lưu trữ, tăng [dung lượng trang web](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) và xoá mục.</span><span class="sxs-lookup"><span data-stu-id="6275e-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="6275e-107">Đảm bảo mục không được [kiểm tra](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) cho người dùng khác.</span><span class="sxs-lookup"><span data-stu-id="6275e-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="6275e-108">Cuối cùng, quản trị viên có thể sử dụng [SharePoint Patterns và thực tiễn](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) chứa một thư viện lệnh PowerShell cho phép bạn thực hiện các hành động quản lý phức tạp như lực xóa các mục cứng đầu.</span><span class="sxs-lookup"><span data-stu-id="6275e-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="6275e-109">Loại bỏ PNP file</span><span class="sxs-lookup"><span data-stu-id="6275e-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="6275e-110">Loại bỏ PNP cặp</span><span class="sxs-lookup"><span data-stu-id="6275e-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="6275e-111">Loại bỏ PNP danh mục</span><span class="sxs-lookup"><span data-stu-id="6275e-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="6275e-112">Loại bỏ PNP danh sách</span><span class="sxs-lookup"><span data-stu-id="6275e-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="6275e-113">Loại bỏ PNP trường (cột)</span><span class="sxs-lookup"><span data-stu-id="6275e-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)