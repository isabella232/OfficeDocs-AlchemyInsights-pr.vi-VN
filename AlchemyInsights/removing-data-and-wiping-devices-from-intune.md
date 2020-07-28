---
title: Xóa dữ liệu và xóa các thiết bị khỏi InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440461"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Xóa dữ liệu và xóa các thiết bị khỏi InTune

Các thiết bị nghỉ hưu và xóa thiết bị hành động từ xa có thể được sử dụng để loại bỏ dữ liệu công ty được quản lý bởi InTune hoặc để thực hiện một Factory Reset và trả lại thiết bị về cài đặt mặc định của nó.

1. Đăng nhập vào Microsoft 365 quản lý thiết bị, và đi đến **thiết**bị  >  **tất cả các thiết bị**.
2. Chọn thiết bị bạn muốn xóa.
3. Chọn loại xóa từ xa mà bạn muốn thực hiện. Nghỉ hưu chỉ xoá thông tin tổ chức, trong khi khăn lau đầy đủ khôi phục thiết bị về cài đặt gốc của nó.
4. Chọn **có** để xác nhận. Cho đến khi kết thúc sạch, trạng thái hành động của thiết bị hiển thị là đang chờ xử lý.</br>
    Sau khi hoàn tất hành động, bạn sẽ không còn thấy thiết bị di động trong danh sách thiết bị được quản lý.

**Lưu ý** Không thể xóa dữ liệu công ty khỏi các thiết bị đã tham gia vào Azure AD.

Để biết chi tiết đầy đủ về hiệu quả của các hành động về hưu và xóa, bao gồm cả những gì được giữ lại và những gì bị xóa, xem [loại bỏ các thiết bị bằng cách sử dụng xóa sạch, rút lui hoặc tự unenrolling thiết bị](https://docs.microsoft.com/intune/devices-wipe).

Để xóa tất cả dữ liệu khỏi thiết bị macOS, xem [xóa tất cả dữ liệu khỏi thiết bị MacOS](https://docs.microsoft.com/intune/device-erase).