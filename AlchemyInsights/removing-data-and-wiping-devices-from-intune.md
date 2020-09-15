---
title: Loại bỏ dữ liệu và các thiết bị xóa khỏi InTune
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
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701305"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Loại bỏ dữ liệu và các thiết bị xóa khỏi InTune

Thiết bị đã rút lui và xóa các hành động từ xa của thiết bị để loại bỏ dữ liệu công ty được quản lý bởi InTune hoặc để thực hiện việc đặt lại nhà máy và trả về thiết bị về thiết đặt mặc định của nó.

1. Đăng nhập vào quản lý thiết bị của Microsoft 365 và đi tới **thiết bị**  >  **tất cả thiết bị**.
2. Chọn thiết bị bạn muốn xóa bỏ.
3. Chọn loại xóa sạch từ xa mà bạn muốn thực hiện. Bỏ ẩn chỉ xóa thông tin tổ chức, trong khi toàn bộ khăn lau khôi phục thiết bị về thiết đặt nhà máy.
4. Chọn **có** để xác nhận. Cho đến khi hoàn tất việc xóa sạch, trạng thái hành động thiết bị sẽ hiển thị là nghỉ hưu đang chờ xử lý.</br>
    Sau khi hoàn thành hành động, bạn sẽ không còn nhìn thấy thiết bị di động trong danh sách thiết bị được quản lý.

**Ghi chú** Không thể loại bỏ dữ liệu công ty khỏi thiết bị đã gia nhập Azure AD.

Để biết chi tiết đầy đủ về hiệu ứng của hành động rút lui và xóa sạch, bao gồm những gì được giữ lại và xóa những gì, hãy xem [loại bỏ các thiết bị bằng cách sử dụng quy trình xóa sạch, rút lui hoặc tự hủy đăng ký thiết bị](https://docs.microsoft.com/intune/devices-wipe).

Để xóa tất cả dữ liệu khỏi thiết bị macOS, hãy xem [xóa tất cả dữ liệu khỏi thiết bị MacOS](https://docs.microsoft.com/intune/device-erase).