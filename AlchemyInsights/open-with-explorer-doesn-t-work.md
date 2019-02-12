---
title: Open Explorer không hoạt động
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: f788c3c626cdeb19970edb59563c59eea60e2992
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906826"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="cea30-102">Open Explorer không hoạt động</span><span class="sxs-lookup"><span data-stu-id="cea30-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="cea30-p101">Nếu **nhìn trong File Explorer** **mở Explorer** hoặc không làm việc đảm bảo rằng các dịch vụ WebClient được thiết lập để **chạy** bằng cách làm theo các bước dưới đây. Ví dụ, nó có thể mất một thời gian dài để mở một thư viện SharePoint hoặc OneDrive khi các dịch vụ không chạy.</span><span class="sxs-lookup"><span data-stu-id="cea30-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="cea30-105">Trong cửa sổ tìm kiếm hộp, loại chạy, chọn các ứng dụng máy tính để bàn chạy, gõ services.msc, và sau đó chọn **nhập**.</span><span class="sxs-lookup"><span data-stu-id="cea30-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="cea30-p102">Di chuyển xuống các dịch vụ WebClient và kiểm tra cột **trạng thái** . Nếu tình trạng dịch vụ WebClient không phải là **chạy**, bấm đúp vào dịch vụ, bấm vào **bắt đầu**, và sau đó nhấp vào **OK**. Kích hoạt dịch vụ, nếu cần thiết, bằng cách chọn hoặc **bằng tay** hoặc **tự động** trong hộp **loại khởi động** .</span><span class="sxs-lookup"><span data-stu-id="cea30-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="cea30-p103">Để khắc phục vấn đề mở File Explorer, nhìn thấy [mở trong Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Khám phá đồng bộ như là một thay thế tốt hơn: [Sync SharePoint các tập tin với các khách hàng mới đồng bộ OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="cea30-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

