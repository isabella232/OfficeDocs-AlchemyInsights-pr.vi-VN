---
title: Mở với Explorer không hoạt động
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694478"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="43df5-102">Mở với Explorer không hoạt động</span><span class="sxs-lookup"><span data-stu-id="43df5-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="43df5-103">Nếu **mở bằng Explorer** hoặc **dạng xem trong file Explorer** không hoạt động đảm bảo dịch vụ webclient được thiết **lập để thực hiện theo dõi** các bước dưới đây.</span><span class="sxs-lookup"><span data-stu-id="43df5-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="43df5-104">Ví dụ: có thể mất nhiều thời gian để mở thư viện SharePoint hoặc OneDrive khi dịch vụ không chạy.</span><span class="sxs-lookup"><span data-stu-id="43df5-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="43df5-105">Trong hộp tìm kiếm Windows, hãy nhập chạy, chọn ứng dụng chạy trên máy tính, nhập Services. msc, rồi chọn **Enter**.</span><span class="sxs-lookup"><span data-stu-id="43df5-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="43df5-106">Cuộn xuống đến dịch vụ WebClient và kiểm tra cột **trạng thái** .</span><span class="sxs-lookup"><span data-stu-id="43df5-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="43df5-107">Nếu trạng thái dịch vụ WebClient không **chạy**, hãy bấm đúp vào dịch vụ, bấm vào **bắt đầu**, rồi bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="43df5-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="43df5-108">Kích hoạt dịch vụ, nếu cần, bằng cách chọn **hướng dẫn sử dụng** hoặc **tự động** trong hộp **kiểu khởi động** .</span><span class="sxs-lookup"><span data-stu-id="43df5-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="43df5-109">Để khắc phục sự cố khi mở trong file Explorer, hãy xem [mở trong Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="43df5-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="43df5-110">Khám phá đồng bộ như một lựa chọn tốt hơn: [đồng bộ các tệp SharePoint với máy khách đồng bộ OneDrive mới](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="43df5-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

