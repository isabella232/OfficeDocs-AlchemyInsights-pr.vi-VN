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
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538511"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="dc477-102">Open Explorer không hoạt động</span><span class="sxs-lookup"><span data-stu-id="dc477-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="dc477-103">Nếu **nhìn trong File Explorer** **mở Explorer** hoặc không làm việc đảm bảo rằng các dịch vụ WebClient được thiết lập để **chạy** bằng cách làm theo các bước dưới đây.</span><span class="sxs-lookup"><span data-stu-id="dc477-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="dc477-104">Ví dụ, nó có thể mất một thời gian dài để mở một thư viện SharePoint hoặc OneDrive khi các dịch vụ không chạy.</span><span class="sxs-lookup"><span data-stu-id="dc477-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="dc477-105">Trong cửa sổ tìm kiếm hộp, loại chạy, chọn các ứng dụng máy tính để bàn chạy, gõ services.msc, và sau đó chọn **nhập**.</span><span class="sxs-lookup"><span data-stu-id="dc477-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="dc477-106">Di chuyển xuống các dịch vụ WebClient và kiểm tra cột **trạng thái** .</span><span class="sxs-lookup"><span data-stu-id="dc477-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="dc477-107">Nếu tình trạng dịch vụ WebClient không phải là **chạy**, bấm đúp vào dịch vụ, bấm vào **bắt đầu**, và sau đó nhấp vào **OK**.</span><span class="sxs-lookup"><span data-stu-id="dc477-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="dc477-108">Kích hoạt dịch vụ, nếu cần thiết, bằng cách chọn hoặc **bằng tay** hoặc **tự động** trong hộp **loại khởi động** .</span><span class="sxs-lookup"><span data-stu-id="dc477-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="dc477-109">Để khắc phục vấn đề mở File Explorer, nhìn thấy [mở trong Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="dc477-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="dc477-110">Khám phá đồng bộ như là một thay thế tốt hơn: [Sync SharePoint các tập tin với các khách hàng mới đồng bộ OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="dc477-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

