---
title: Khắc phục sự cố khi mở bằng Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659080"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="0eb1d-102">Khắc phục sự cố khi mở với Explorer</span><span class="sxs-lookup"><span data-stu-id="0eb1d-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="0eb1d-103">Khắc phục các sự cố phổ biến khi mở một thư viện tài liệu trong SharePoint hoặc OneDrive bằng lệnh **mở với Explorer** :</span><span class="sxs-lookup"><span data-stu-id="0eb1d-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="0eb1d-104">Sử dụng Internet Explorer 10 hoặc Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="0eb1d-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="0eb1d-105">**Mở với Explorer** không tương thích với Microsoft Edge, Google Chrome, Firefox và những người khác.</span><span class="sxs-lookup"><span data-stu-id="0eb1d-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="0eb1d-106">**Mở với Explorer** đã bị vô hiệu hóa trong tất cả các trình duyệt, ngoại trừ Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="0eb1d-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="0eb1d-107">**Mở bằng Explorer** không sẵn dùng trong trải nghiệm hiện đại cho thư viện SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0eb1d-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="0eb1d-108">Sử dụng **dạng xem trong file Explorer** thay vào đó.</span><span class="sxs-lookup"><span data-stu-id="0eb1d-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="0eb1d-109">Chọn dạng xem **tùy chọn xem** \> **trong file Explorer**.</span><span class="sxs-lookup"><span data-stu-id="0eb1d-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="0eb1d-110">Xem trong file Explorer không tương thích với Microsoft Edge, Google Chrome, Firefox và những người khác.</span><span class="sxs-lookup"><span data-stu-id="0eb1d-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="0eb1d-111">**Xem trong file Explorer** chỉ sẵn dùng trong Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="0eb1d-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="0eb1d-112">Đảm bảo rằng dịch vụ WebClient đang chạy.</span><span class="sxs-lookup"><span data-stu-id="0eb1d-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="0eb1d-113">Trong hộp tìm kiếm Windows, hãy nhập chạy, chọn ứng dụng chạy trên máy tính, nhập Services. msc, rồi nhấn Enter.</span><span class="sxs-lookup"><span data-stu-id="0eb1d-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="0eb1d-114">Cuộn xuống đến dịch vụ WebClient và đảm bảo cột **trạng thái** sẽ hiển thị "đang chạy".</span><span class="sxs-lookup"><span data-stu-id="0eb1d-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="0eb1d-115">Nếu không, hãy bấm đúp vào dịch vụ, bấm vào **bắt đầu**, rồi bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="0eb1d-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="0eb1d-116">(Trước tiên, bạn có thể phải bật dịch vụ bằng cách chọn **thủ** công hoặc **tự động** trong hộp **kiểu khởi động** .)</span><span class="sxs-lookup"><span data-stu-id="0eb1d-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="0eb1d-117">Mở một thư viện trong file Explorer có ích nếu bạn cần sao chép hoặc di chuyển nhiều tệp và thư mục một lần, nhưng nếu bạn muốn làm việc thường xuyên trong thư viện, chúng tôi khuyên bạn nên đồng bộ nó.</span><span class="sxs-lookup"><span data-stu-id="0eb1d-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="0eb1d-118">Để khắc phục sự cố khi mở trong file Explorer, hãy xem [mở trong Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="0eb1d-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="0eb1d-119">Để biết thông tin về việc thiết lập đồng bộ, hãy xem [đồng bộ các tệp SharePoint với máy khách đồng bộ OneDrive mới](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="0eb1d-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="0eb1d-120">Vui lòng xem bài viết [cách dùng lệnh "mở bằng Explorer" để khắc phục sự cố trong SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="0eb1d-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

