---
title: Khôi phục tệp hoặc thư mục đã xóa
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 2702837bff2c0a465dde2c090a44e02747cc85ec
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051087"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="fe5d3-102">Khôi phục tệp hoặc thư mục đã xóa</span><span class="sxs-lookup"><span data-stu-id="fe5d3-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="fe5d3-103">SharePoint Online giữ lại bản sao lưu của tất cả nội dung cho 14 ngày bổ sung ngoài thực tế xóa.</span><span class="sxs-lookup"><span data-stu-id="fe5d3-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="fe5d3-104">Nếu không thể khôi phục nội dung qua thùng rác hoặc khôi phục tệp, quản trị viên có thể liên hệ với bộ hỗ trợ của Microsoft để yêu cầu khôi phục bất kỳ thời gian nào trong cửa sổ 14 ngày.</span><span class="sxs-lookup"><span data-stu-id="fe5d3-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="fe5d3-105">Phục hồi từ sao lưu chỉ có thể được hoàn thành cho các bộ sưu tập trang web hoặc các trang web phụ, không phải cho các tập tin cụ thể, danh sách, hoặc thư viện.</span><span class="sxs-lookup"><span data-stu-id="fe5d3-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="fe5d3-106">Khi bạn xóa một mục hoặc trang web khỏi SharePoint, nó sẽ không bị xóa ngay lập tức.</span><span class="sxs-lookup"><span data-stu-id="fe5d3-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="fe5d3-107">Các mục đã xóa đi vào thùng rác trong một khoảng thời gian.</span><span class="sxs-lookup"><span data-stu-id="fe5d3-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="fe5d3-108">Trong thời gian đó, bạn có thể khôi phục các mục bạn đã xóa vào vị trí ban đầu của họ.</span><span class="sxs-lookup"><span data-stu-id="fe5d3-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="fe5d3-109">Để biết thêm thông tin, xin vui lòng truy cập vào các liên kết dưới đây.</span><span class="sxs-lookup"><span data-stu-id="fe5d3-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="fe5d3-110">[Khôi phục các mục trong thùng rác của trang web SharePoint](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span><span class="sxs-lookup"><span data-stu-id="fe5d3-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="fe5d3-111">Khôi phục các tệp hoặc thư mục đã xóa trong OneDrive</span><span class="sxs-lookup"><span data-stu-id="fe5d3-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="fe5d3-112">Khôi phục bộ sưu tập trang web đã xóa (bao gồm nhóm, giao tiếp và các trang web khác)</span><span class="sxs-lookup"><span data-stu-id="fe5d3-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="fe5d3-113">Khôi phục trang web OneDrive đã xóa</span><span class="sxs-lookup"><span data-stu-id="fe5d3-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="fe5d3-114">Đối với số lượng lớn thùng rác hành động, quản trị viên có thể xem xét sử dụng [SharePoint trực tuyến PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="fe5d3-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="fe5d3-115">**Tính năng khôi phục tệp**</span><span class="sxs-lookup"><span data-stu-id="fe5d3-115">**Files Restore feature**</span></span>

<span data-ttu-id="fe5d3-116">Nếu nhiều tệp OneDrive hoặc SharePoint của bạn bị xóa, ghi đè, bị hỏng hoặc bị nhiễm phần mềm độc hại, bạn có thể khôi phục toàn bộ thư viện OneDrive hoặc SharePoint của bạn đến một thời gian trước bằng cách sử dụng tính năng khôi phục tệp.</span><span class="sxs-lookup"><span data-stu-id="fe5d3-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="fe5d3-117">Khôi phục thư viện OneDrive</span><span class="sxs-lookup"><span data-stu-id="fe5d3-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="fe5d3-118">Khôi phục thư viện tài liệu</span><span class="sxs-lookup"><span data-stu-id="fe5d3-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

