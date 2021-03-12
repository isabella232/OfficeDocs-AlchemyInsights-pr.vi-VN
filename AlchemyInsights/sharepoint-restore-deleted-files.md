---
title: Khôi phục tệp hoặc thư mục đã xóa
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 8c7ce48f50b5c933ea15c23a486b99ad7a7f4d79
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707544"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="57656-102">Khôi phục tệp hoặc thư mục đã xóa</span><span class="sxs-lookup"><span data-stu-id="57656-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="57656-103">SharePoint Online giữ lại bản sao lưu của tất cả nội dung trong 14 ngày bổ sung ngoài việc xóa thực tế.</span><span class="sxs-lookup"><span data-stu-id="57656-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="57656-104">Nếu không thể khôi phục nội dung qua thùng rác hoặc khôi phục tệp, người quản trị có thể liên hệ với bộ phận hỗ trợ của Microsoft để yêu cầu khôi phục bất kỳ lúc nào trong cửa sổ 14 ngày.</span><span class="sxs-lookup"><span data-stu-id="57656-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="57656-105">Khôi phục từ các sao lưu chỉ có thể hoàn thành đối với tuyển tập site hoặc các site con, không đối với các tệp, danh sách hoặc thư viện cụ thể.</span><span class="sxs-lookup"><span data-stu-id="57656-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="57656-106">Khi bạn xóa một mục hoặc site khỏi SharePoint, nó không được loại bỏ ngay lập tức.</span><span class="sxs-lookup"><span data-stu-id="57656-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="57656-107">Các mục đã xóa đi vào thùng rác trong một khoảng thời gian.</span><span class="sxs-lookup"><span data-stu-id="57656-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="57656-108">Trong thời gian đó, bạn có thể khôi phục các mục mà bạn đã xóa vào vị trí ban đầu của họ.</span><span class="sxs-lookup"><span data-stu-id="57656-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="57656-109">Để biết thêm thông tin, vui lòng truy cập vào các nối kết dưới đây.</span><span class="sxs-lookup"><span data-stu-id="57656-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="57656-110">[Khôi phục các mục trong thùng rác của một site SharePoint](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be).</span><span class="sxs-lookup"><span data-stu-id="57656-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be).</span></span>

[<span data-ttu-id="57656-111">Khôi phục tệp hoặc thư mục đã xóa trong OneDrive</span><span class="sxs-lookup"><span data-stu-id="57656-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="57656-112">Khôi phục tuyển tập trang đã xóa (bao gồm nhóm, liên lạc và các site khác)</span><span class="sxs-lookup"><span data-stu-id="57656-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="57656-113">Khôi phục site OneDrive đã xóa</span><span class="sxs-lookup"><span data-stu-id="57656-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="57656-114">Đối với các hành động thùng rác hàng loạt, người quản trị có thể cân nhắc việc sử dụng [SharePoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="57656-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="57656-115">**Tính năng khôi phục tệp**</span><span class="sxs-lookup"><span data-stu-id="57656-115">**Files Restore feature**</span></span>

<span data-ttu-id="57656-116">Nếu rất nhiều các tệp OneDrive hoặc SharePoint bị xóa, ghi đè, bị lỗi hoặc bị phần mềm độc hại, bạn có thể khôi phục toàn bộ thư viện OneDrive hoặc SharePoint của mình vào một thời gian trước đó bằng cách sử dụng tính năng khôi phục tệp.</span><span class="sxs-lookup"><span data-stu-id="57656-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="57656-117">Khôi phục thư viện OneDrive</span><span class="sxs-lookup"><span data-stu-id="57656-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="57656-118">Khôi phục thư viện tài liệu</span><span class="sxs-lookup"><span data-stu-id="57656-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

