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
# <a name="open-with-explorer-isnt-working"></a>Mở bằng Explorer không hoạt động

Nếu **mở với Explorer** hoặc **xem trong file Explorer** không hoạt động đảm bảo rằng dịch vụ webclient được thiết lập để **chạy** bằng cách làm theo các bước dưới đây. Ví dụ: có thể mất nhiều thời gian để mở thư viện SharePoint hoặc OneDrive khi dịch vụ không chạy. 
  
1. Trong hộp tìm kiếm của Windows, nhập chạy, chọn ứng dụng chạy trên máy tính, gõ Services. msc, và sau đó chọn **Enter**.
    
2. Cuộn xuống dịch vụ WebClient và kiểm tra cột **trạng thái** . Nếu trạng thái dịch vụ WebClient không **chạy**, bấm đúp vào dịch vụ, bấm **bắt đầu**, và sau đó bấm **OK**. Kích hoạt dịch vụ, nếu cần thiết, bằng cách chọn bằng **tay** hoặc **tự động** trong hộp **loại khởi động** . 
    
> [!NOTE]
> Để khắc phục sự cố mở trong file Explorer, hãy xem [mở trong Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Khám phá đồng bộ để thay thế tốt hơn: [đồng bộ hóa SharePoint tệp với khách hàng đồng bộ OneDrive mới](https://go.microsoft.com/fwlink/?linkid=871666). 
  

