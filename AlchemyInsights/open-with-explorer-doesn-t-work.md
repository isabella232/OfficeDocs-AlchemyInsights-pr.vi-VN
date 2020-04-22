---
title: Mở bằng Explorer không hoạt động
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713056"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="13668-102">Mở bằng Explorer không hoạt động</span><span class="sxs-lookup"><span data-stu-id="13668-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="13668-103">Nếu **mở với Explorer** hoặc **xem trong file Explorer** không hoạt động đảm bảo rằng dịch vụ webclient được thiết lập để **chạy** bằng cách làm theo các bước dưới đây.</span><span class="sxs-lookup"><span data-stu-id="13668-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="13668-104">Ví dụ: có thể mất nhiều thời gian để mở thư viện SharePoint hoặc OneDrive khi dịch vụ không chạy.</span><span class="sxs-lookup"><span data-stu-id="13668-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="13668-105">Trong hộp tìm kiếm của Windows, nhập chạy, chọn ứng dụng chạy trên máy tính, gõ Services. msc, và sau đó chọn **Enter**.</span><span class="sxs-lookup"><span data-stu-id="13668-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="13668-106">Cuộn xuống dịch vụ WebClient và kiểm tra cột **trạng thái** .</span><span class="sxs-lookup"><span data-stu-id="13668-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="13668-107">Nếu trạng thái dịch vụ WebClient không **chạy**, bấm đúp vào dịch vụ, bấm **bắt đầu**, và sau đó bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="13668-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="13668-108">Kích hoạt dịch vụ, nếu cần thiết, bằng cách chọn bằng **tay** hoặc **tự động** trong hộp **loại khởi động** .</span><span class="sxs-lookup"><span data-stu-id="13668-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="13668-109">Để khắc phục sự cố mở trong file Explorer, hãy xem [mở trong Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="13668-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="13668-110">Khám phá đồng bộ để thay thế tốt hơn: [đồng bộ hóa SharePoint tệp với khách hàng đồng bộ OneDrive mới](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="13668-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

