---
title: Làm việc với các ứng dụng iOS VPP ID quy tắc 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719979"
---
# <a name="working-with-ios-vpp-applications"></a>Làm việc với các ứng dụng iOS VPP

Đọc [cách quản lý các ứng dụng iOS mua thông qua chương trình mua ổ đĩa với Microsoft InTune](https://docs.microsoft.com/intune/vpp-apps-ios) để tìm hiểu về các tính năng, ràng buộc và các bước để sử dụng chương trình mua và hỗ trợ của Apple trong Microsoft InTune.
  
 **Các vấn đề thường gặp:** "Tôi đã gán một ứng dụng iOS VPP cho người dùng của tôi, nhưng việc cài đặt không thành công."
  
- Điều này có thể xảy ra nếu một mã thông báo VPP duy nhất được sử dụng trên nhiều nhà cung cấp quản lý thiết bị di động. Thẻ VPP từ Apple chỉ có thể được sử dụng với một nhà cung cấp. Nếu bạn sử dụng một thẻ VPP với nhiều nhà cung cấp, bạn phải tải lên lại mã thông báo để InTune.

- Quá trình cài đặt cũng có thể thất bại nếu tổng số cài đặt vượt quá số lượng giấy phép. Để xem báo cáo sử dụng cho giấy phép của bạn, hãy chuyển đến trang \> **giấy phép** ứng dụng **dành cho thiết bị di động InTune** . Để tìm hiểu cách lấy lại giấy phép sử dụng, hãy xem [bài viết này.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
