---
title: Gỡ rối các vấn đề bằng cách sử dụng mở Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390629"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="b052a-102">Sửa các vấn đề mở Explorer</span><span class="sxs-lookup"><span data-stu-id="b052a-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="b052a-103">Sửa chữa các vấn đề thường gặp với việc mở một thư viện tài liệu trong SharePoint hoặc OneDrive sử dụng lệnh **Open Explorer** :</span><span class="sxs-lookup"><span data-stu-id="b052a-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="b052a-104">Sử dụng Internet Explorer 10 hoặc Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="b052a-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="b052a-105">**Open Explorer** không tương thích với Microsoft Edge, Google Chrome, Firefox và những người khác.</span><span class="sxs-lookup"><span data-stu-id="b052a-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="b052a-106">**Open Explorer** bị vô hiệu hóa trong tất cả các trình duyệt ngoại trừ Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="b052a-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="b052a-107">**Open Explorer** không phải là có sẵn trong những kinh nghiệm hiện đại cho các thư viện SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b052a-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="b052a-108">Thay vì sử dụng **chế độ xem trong File Explorer** .</span><span class="sxs-lookup"><span data-stu-id="b052a-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="b052a-109">Chọn **tùy chọn View** \> **xem trong File Explorer**.</span><span class="sxs-lookup"><span data-stu-id="b052a-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="b052a-110">Chế độ xem trong File Explorer không phải là tương thích với Microsoft Edge, Google Chrome, Firefox và những người khác.</span><span class="sxs-lookup"><span data-stu-id="b052a-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="b052a-111">**Chế độ xem trong File Explorer** trong chỉ có trong Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="b052a-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="b052a-112">Đảm bảo rằng các dịch vụ WebClient đang chạy.</span><span class="sxs-lookup"><span data-stu-id="b052a-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="b052a-113">Trong hộp tìm kiếm của Windows, gõ run, chọn các ứng dụng máy tính để bàn chạy, gõ services.msc, và sau đó nhấn Enter.</span><span class="sxs-lookup"><span data-stu-id="b052a-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="b052a-114">Cuộn xuống WebClient dịch vụ và đảm bảo rằng cột **trạng thái** sẽ hiển thị "Chạy."</span><span class="sxs-lookup"><span data-stu-id="b052a-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="b052a-115">Nếu không, bấm đúp vào dịch vụ, bấm vào **bắt đầu**, và sau đó nhấp vào **OK**.</span><span class="sxs-lookup"><span data-stu-id="b052a-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="b052a-116">(Bạn có thể cần để lần đầu tiên kích hoạt dịch vụ bằng cách chọn hoặc **bằng tay** hoặc **tự động** trong hộp **loại khởi động** .)</span><span class="sxs-lookup"><span data-stu-id="b052a-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="b052a-117">Mở một thư viện trong File Explorer là hữu ích nếu bạn cần để sao chép hoặc di chuyển nhiều tập tin và thư mục sau khi, nhưng nếu bạn muốn thường xuyên làm việc trong thư viện, chúng tôi khuyên bạn nên đồng bộ hoá nó.</span><span class="sxs-lookup"><span data-stu-id="b052a-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="b052a-118">Để khắc phục vấn đề mở File Explorer, nhìn thấy [mở trong Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="b052a-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="b052a-119">Thông tin về việc thiết lập đồng bộ, xem [tập tin Sync SharePoint với khách hàng mới đồng bộ OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="b052a-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="b052a-120">Xin vui lòng xem bài viết [làm thế nào để sử dụng lệnh "mở với Explorer" khắc phục sự cố các vấn đề trong SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) cho biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="b052a-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

