---
title: Khôi phục đã bị xóa file hoặc thư mục
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 604690e62f09b7ca0618c4a581605e22f19a7732
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507473"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="892b2-102">Khôi phục đã bị xóa file hoặc thư mục</span><span class="sxs-lookup"><span data-stu-id="892b2-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="892b2-103">SharePoint Online giữ bản sao lưu của tất cả nội dung trong 14 ngày bổ sung vượt ra ngoài thực tế xóa.</span><span class="sxs-lookup"><span data-stu-id="892b2-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="892b2-104">Nếu nội dung không thể khôi phục thông qua thùng rác hoặc khôi phục tập tin, người quản trị có thể liên hệ với Microsoft Support để yêu cầu một khôi phục lại bất kỳ thời điểm nào trong cửa sổ 14 ngày.</span><span class="sxs-lookup"><span data-stu-id="892b2-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="892b2-105">Phục hồi từ bản sao lưu chỉ có thể được hoàn thành cho bộ sưu tập trang web hoặc các trang phụ, không cho các tập tin cụ thể, danh sách hoặc thư viện.</span><span class="sxs-lookup"><span data-stu-id="892b2-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="892b2-106">Khi bạn xoá một mục hoặc trang web từ Sharepoint, nó không phải là ngay lập tức bị loại bỏ.</span><span class="sxs-lookup"><span data-stu-id="892b2-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="892b2-107">Khoản mục đã xóa đi vào thùng rác cho một khoảng thời gian.</span><span class="sxs-lookup"><span data-stu-id="892b2-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="892b2-108">Trong thời gian đó, bạn có thể khôi phục lại các khoản mục bạn đã xoá vị trí ban đầu của họ.</span><span class="sxs-lookup"><span data-stu-id="892b2-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="892b2-109">Để biết thêm chi tiết, xin vui lòng truy cập vào liên kết dưới đây.</span><span class="sxs-lookup"><span data-stu-id="892b2-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="892b2-110">[Khôi phục các khoản mục trong thùng rác của một trang web SharePoint](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="892b2-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

[<span data-ttu-id="892b2-111">Phục hồi xóa các tập tin hoặc thư mục trong OneDrive</span><span class="sxs-lookup"><span data-stu-id="892b2-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="892b2-112">Khôi phục lại một bộ sưu tập trang web đã xóa (bao gồm cả nhóm, giao tiếp và các trang web khác)</span><span class="sxs-lookup"><span data-stu-id="892b2-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="892b2-113">Khôi phục lại một trang web đã xóa OneDrive</span><span class="sxs-lookup"><span data-stu-id="892b2-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="892b2-114">Đối với số lượng lớn recycle bin hành động, quản trị viên có thể xem xét sử dụng [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="892b2-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="892b2-115">**Tính năng khôi phục lại các tập tin**</span><span class="sxs-lookup"><span data-stu-id="892b2-115">**Files Restore feature**</span></span>

<span data-ttu-id="892b2-116">Nếu nhiều của bạn tập tin OneDrive hoặc SharePoint có được xóa bỏ, ghi đè, bị hỏng hoặc nhiễm phần mềm độc hại, bạn có thể khôi phục lại thư viện toàn bộ OneDrive hoặc SharePoint của bạn một thời gian trước đó bằng cách sử dụng tính năng khôi phục lại các tập tin.</span><span class="sxs-lookup"><span data-stu-id="892b2-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="892b2-117">Khôi phục thư viện OneDrive</span><span class="sxs-lookup"><span data-stu-id="892b2-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="892b2-118">Khôi phục thư viện tài liệu</span><span class="sxs-lookup"><span data-stu-id="892b2-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a?ui=en-US&amp;rs=en-US&amp;ad=US.)

