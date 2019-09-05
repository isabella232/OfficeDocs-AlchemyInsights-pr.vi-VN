---
title: Khắc phục sự cố sử dụng mở với Explorer
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
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742755"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="09d07-102">Khắc phục sự cố với Open With Explorer</span><span class="sxs-lookup"><span data-stu-id="09d07-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="09d07-103">Khắc phục sự cố thường gặp với việc mở thư viện tài liệu trong SharePoint hoặc OneDrive bằng lệnh **mở Explorer** :</span><span class="sxs-lookup"><span data-stu-id="09d07-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="09d07-104">Sử dụng Internet Explorer 10 hoặc Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="09d07-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="09d07-105">**Mở bằng Explorer** không tương thích với Microsoft Edge, Google Chrome, Firefox và những người khác.</span><span class="sxs-lookup"><span data-stu-id="09d07-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="09d07-106">**Mở với Explorer** bị vô hiệu hoá trong tất cả các trình duyệt ngoại trừ Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="09d07-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="09d07-107">**Mở bằng Explorer** không có trong trải nghiệm hiện đại cho thư viện SharePoint.</span><span class="sxs-lookup"><span data-stu-id="09d07-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="09d07-108">Sử dụng **dạng xem trong file Explorer** thay thế.</span><span class="sxs-lookup"><span data-stu-id="09d07-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="09d07-109">Chọn xem **tùy chọn** \> **xem trong file Explorer**.</span><span class="sxs-lookup"><span data-stu-id="09d07-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="09d07-110">Xem trong file Explorer không tương thích với Microsoft Edge, Google Chrome, Firefox và những người khác.</span><span class="sxs-lookup"><span data-stu-id="09d07-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="09d07-111">**Xem trong file Explorer** chỉ có sẵn trong Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="09d07-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="09d07-112">Đảm bảo rằng dịch vụ WebClient đang chạy.</span><span class="sxs-lookup"><span data-stu-id="09d07-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="09d07-113">Trong hộp tìm kiếm của Windows, nhập chạy, chọn ứng dụng Run Desktop, gõ Services. msc, và sau đó nhấn Enter.</span><span class="sxs-lookup"><span data-stu-id="09d07-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="09d07-114">Cuộn xuống dịch vụ WebClient và đảm bảo rằng cột **trạng thái** Hiển thị "đang chạy."</span><span class="sxs-lookup"><span data-stu-id="09d07-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="09d07-115">Nếu không, bấm đúp vào dịch vụ, bấm **bắt đầu**, và sau đó bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="09d07-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="09d07-116">(Bạn có thể cần phải kích hoạt dịch vụ trước tiên bằng cách chọn **hướng dẫn sử dụng** hoặc **tự động** trong hộp **loại khởi động** .)</span><span class="sxs-lookup"><span data-stu-id="09d07-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="09d07-117">Mở một thư viện trong file Explorer là tiện dụng nếu bạn cần sao chép hoặc di chuyển nhiều tệp và thư mục một lần, nhưng nếu bạn muốn thường xuyên làm việc trong thư viện, chúng tôi khuyên bạn nên đồng bộ hóa nó.</span><span class="sxs-lookup"><span data-stu-id="09d07-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="09d07-118">Để khắc phục sự cố mở trong file Explorer, hãy xem [mở trong Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="09d07-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="09d07-119">Để biết thông tin về thiết lập đồng bộ hóa, [hãy xem đồng bộ hóa tệp SharePoint với khách hàng đồng bộ OneDrive mới](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="09d07-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="09d07-120">Vui lòng xem bài viết [cách sử dụng lệnh "mở bằng Explorer" để khắc phục sự cố trong SharePoint trực tuyến để](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="09d07-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

