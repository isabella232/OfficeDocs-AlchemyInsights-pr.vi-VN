---
title: Tính năng Mở bằng Explorer không hoạt động
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
ms.openlocfilehash: 2ba6f08b40dd194bf1ffd9a455a134a2fc553b51
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321883"
---
# <a name="open-with-explorer-isnt-working"></a>Tính năng Mở bằng Explorer không hoạt động

Nếu **Mở bằng Explorer hoặc** Xem trong File **Explorer** không hoạt động,  hãy đảm bảo dịch vụ WebClient được đặt thành Chạy bằng cách làm theo các bước dưới đây. Ví dụ: có thể mất nhiều thời gian để mở một thư viện SharePoint hoặc OneDrive khi dịch vụ hiện không chạy. 
  
1. Trong hộp tìm Windows, nhập Run, chọn ứng dụng Run trên máy tính, nhập services.msc, rồi chọn **Enter**.
    
2. Cuộn xuống dịch vụ WebClient và kiểm tra **cột Trạng** thái. Nếu trạng thái dịch vụ WebClient không Chạy **,** hãy bấm đúp vào dịch vụ, bấm vào **Bắt đầu**, rồi bấm **vào OK.** Bật dịch vụ, nếu cần, bằng cách chọn Thủ **công hoặc** **Tự động** trong hộp **Kiểu khởi** động. 
    
**Ghi chú**: Để khắc phục sự cố mở trong File Explorer, hãy [xem Mở trong Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Khám phá cách đồng bộ như một giải pháp thay thế tốt hơn: Đồng bộ [tệp SharePoint với máy khách Đồng bộ OneDrive mới.](https://go.microsoft.com/fwlink/?linkid=871666) 
  

