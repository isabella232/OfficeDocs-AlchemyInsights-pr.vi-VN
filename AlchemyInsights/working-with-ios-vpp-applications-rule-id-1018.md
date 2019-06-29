---
title: Làm việc với iOS VPP ứng dụng quy tắc Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 58471f22ce78be1b40d3330a76a92d811819849d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364896"
---
# <a name="working-with-ios-vpp-applications"></a>Làm việc với iOS VPP ứng dụng

Đọc [làm thế nào để quản lý các ứng dụng iOS mua thông qua một chương trình mua hàng khối lượng với Microsoft dành](https://docs.microsoft.com/intune/vpp-apps-ios) để tìm hiểu về tính năng, những hạn chế, và các bước để làm cho việc sử dụng chương trình mua khối lượng của Apple và hỗ trợ cho nó trong Microsoft Intune.
  
 **Những vấn đề chung:** "Tôi chỉ định một ứng dụng VPP iOS để người dùng của tôi, nhưng tiến trình cài đặt thất bại."
  
- Điều này có thể xảy ra nếu một mã thông báo VPP duy nhất được sử dụng trên nhiều thiết bị di động quản lý nhà cung cấp. VPP thẻ từ Apple chỉ có thể được sử dụng với một trong những nhà cung cấp. Nếu bạn đã sử dụng một mã thông báo VPP với nhiều nhà cung cấp, bạn lại phải tải lên mã thông báo để dành.

- Việc cài đặt có thể cũng không thành công nếu tổng số cài đặt vượt quá số lượng giấy phép. Để xem báo cáo sử dụng cho các giấy phép của bạn, hãy vào **ứng dụng điện thoại di động dành** \> **giấy phép ứng dụng** trang. Để tìm hiểu làm thế nào để thu hồi giấy phép sử dụng, hãy xem [bài viết này.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
