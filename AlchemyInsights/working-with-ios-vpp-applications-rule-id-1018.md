---
title: Làm việc với quy tắc ứng dụng iOS VPP 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688968"
---
# <a name="working-with-ios-vpp-applications"></a>Làm việc với các ứng dụng iOS VPP

Đọc [cách quản lý các ứng dụng iOS được mua thông qua chương trình mua âm lượng với Microsoft InTune](https://docs.microsoft.com/intune/vpp-apps-ios) để tìm hiểu về các tính năng, ràng buộc và các bước để làm cho việc sử dụng chương trình mua âm lượng của Apple và hỗ trợ cho nó trong Microsoft InTune.
  
 Các **vấn đề chung:** "Tôi đã gán một ứng dụng iOS VPP cho người dùng của mình, nhưng quá trình cài đặt không thành công."
  
- Điều này có thể xảy ra nếu một mã thông báo VPP đơn được dùng trên nhiều nhà cung cấp dịch vụ quản lý thiết bị di động. Các thẻ VPP từ Apple chỉ có thể sử dụng với một nhà cung cấp. Nếu bạn đã sử dụng một mã thông báo VPP với nhiều nhà cung cấp, bạn phải tải lên lại mã thông báo để InTune.

- Quá trình cài đặt cũng có thể không thành công nếu tổng số lượng bản cài đặt vượt quá số lượng giấy phép. Để xem báo cáo sử dụng cho giấy phép của bạn, **Intune Mobile apps** hãy đi đến \> trang **giấy phép ứng** dụng InTune trên thiết bị di động. Để tìm hiểu cách đòi hỏi giấy phép đang sử dụng, hãy xem [bài viết này.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
