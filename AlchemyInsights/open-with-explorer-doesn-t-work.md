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
# <a name="open-with-explorer-isnt-working"></a>Open Explorer không hoạt động

Nếu **nhìn trong File Explorer** **mở Explorer** hoặc không làm việc đảm bảo rằng các dịch vụ WebClient được thiết lập để **chạy** bằng cách làm theo các bước dưới đây. Ví dụ, nó có thể mất một thời gian dài để mở một thư viện SharePoint hoặc OneDrive khi các dịch vụ không chạy. 
  
1. Trong cửa sổ tìm kiếm hộp, loại chạy, chọn các ứng dụng máy tính để bàn chạy, gõ services.msc, và sau đó chọn **nhập**.
    
2. Di chuyển xuống các dịch vụ WebClient và kiểm tra cột **trạng thái** . Nếu tình trạng dịch vụ WebClient không phải là **chạy**, bấm đúp vào dịch vụ, bấm vào **bắt đầu**, và sau đó nhấp vào **OK**. Kích hoạt dịch vụ, nếu cần thiết, bằng cách chọn hoặc **bằng tay** hoặc **tự động** trong hộp **loại khởi động** . 
    
> [!NOTE]
> Để khắc phục vấn đề mở File Explorer, nhìn thấy [mở trong Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Khám phá đồng bộ như là một thay thế tốt hơn: [Sync SharePoint các tập tin với các khách hàng mới đồng bộ OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

