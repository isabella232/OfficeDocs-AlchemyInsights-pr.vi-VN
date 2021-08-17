---
title: Làm việc với Id Quy tắc Ứng dụng VPP của iOS 1018
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
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083036"
---
# <a name="working-with-ios-vpp-applications"></a>Làm việc với ứng dụng VPP của iOS

Đọc mục Cách quản lý các ứng dụng iOS đã mua thông qua chương trình mua hàng số lượng lớn với Microsoft Intune để tìm hiểu về các tính năng, ràng buộc và các bước sử dụng Chương trình Mua Hàng Lớn của Apple và sự hỗ trợ của chương trình này trong [Microsoft Intune.](https://docs.microsoft.com/intune/vpp-apps-ios)
  
 **Sự cố Phổ biến:** "Tôi đã gán ứng dụng VPP iOS cho người dùng của mình, nhưng quá trình cài đặt không thành công".
  
- Điều này có thể xảy ra nếu một mã thông báo VPP được sử dụng cho nhiều nhà cung cấp dịch vụ quản lý thiết bị di động. Mã thông báo VPP từ Apple chỉ có thể được sử dụng với một nhà cung cấp. Nếu bạn đã sử dụng mã thông báo VPP với nhiều nhà cung cấp, bạn phải tải mã thông báo đó lên Intune lại.

- Quá trình cài đặt cũng có thể không thành công nếu tổng số bản cài đặt vượt quá số giấy phép. Để xem báo cáo sử dụng giấy phép của bạn, hãy đi đến trang Giấy phép ứng dụng **Intune** \>  Mobile. Để tìm hiểu cách thu hồi giấy phép đang sử dụng, hãy xem bài [viết này.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
