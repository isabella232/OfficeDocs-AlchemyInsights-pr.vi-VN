---
title: Loại bỏ dữ liệu và xóa thiết bị khỏi Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: 92673c4a2a0e0faa98d3ade5ca1f6aa687d4c94a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331063"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Loại bỏ dữ liệu và xóa thiết bị khỏi Intune

Bạn có thể sử dụng hành động từ xa Xóa thiết bị và Xóa thiết bị để loại bỏ dữ liệu công ty do Intune quản lý hoặc để thực hiện đặt lại về cài đặt gốc và đưa thiết bị về cài đặt mặc định.

1. Đăng nhập vào Microsoft 365 lý Thiết bị và đi đến Thiết bị **Tất cả**  >  **Thiết bị**.
2. Chọn thiết bị bạn muốn xóa.
3. Chọn kiểu xóa từ xa mà bạn muốn thực hiện. Ngừng hoạt động chỉ xóa thông tin của tổ chức, trong khi xóa toàn bộ dữ liệu sẽ khôi phục thiết bị về cài đặt tại nhà máy.
4. Chọn **Có để** xác nhận. Cho đến khi quá trình xóa hoàn tất, trạng thái hành động Thiết bị hiển thị là *Đang chờ xử lý Ngừng sử dụng*.
    Sau khi hoàn tất hành động, bạn sẽ không còn thấy thiết bị di động trong danh sách thiết bị được quản lý.

**Lưu ý:** Không thể loại bỏ dữ liệu công ty khỏi các thiết bị ĐÃ THAM GIA Azure AD. 

Để biết chi tiết đầy đủ về tác động của hành động Ngừng sử dụng và Xóa, bao gồm nội dung được giữ lại và nội dung bị xóa, hãy xem tài liệu sau đây:

- [Loại bỏ thiết bị bằng cách sử dụng xóa sạch, ngừng sử dụng hoặc bỏ kiểm soát thiết bị theo cách thủ công](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Cách chỉ xóa dữ liệu công ty khỏi các ứng dụng do Intune quản lý](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Xóa tất cả dữ liệu khỏi thiết bị macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).