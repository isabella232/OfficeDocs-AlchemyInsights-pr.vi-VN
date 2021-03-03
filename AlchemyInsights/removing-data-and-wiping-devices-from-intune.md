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
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416335"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Loại bỏ dữ liệu và các thiết bị xóa khỏi InTune

Thiết bị đã rút lui và xóa các hành động từ xa của thiết bị để loại bỏ dữ liệu công ty được quản lý bởi InTune hoặc để thực hiện việc đặt lại nhà máy và trả về thiết bị về thiết đặt mặc định của nó.

1. Đăng nhập vào quản lý thiết bị của Microsoft 365 và đi tới **thiết bị**  >  **tất cả thiết bị**.
2. Chọn thiết bị bạn muốn xóa bỏ.
3. Chọn loại xóa sạch từ xa mà bạn muốn thực hiện. Bỏ ẩn chỉ xóa thông tin tổ chức, trong khi toàn bộ khăn lau khôi phục thiết bị về thiết đặt nhà máy.
4. Chọn **có** để xác nhận. Cho đến khi hoàn tất việc xóa sạch, trạng thái hành động thiết bị sẽ hiển thị là *nghỉ hưu đang chờ xử* lý.
    Sau khi hoàn thành hành động, bạn sẽ không còn nhìn thấy thiết bị di động trong danh sách thiết bị được quản lý.

> [!NOTE]
> Không thể loại bỏ dữ liệu công ty khỏi thiết bị đã gia nhập Azure AD. 

Để biết chi tiết đầy đủ về hiệu ứng của hành động rút lui và xóa sạch, bao gồm những gì được giữ lại và xóa những gì, hãy xem tài liệu hướng dẫn sau:

- [Loại bỏ các thiết bị bằng cách sử dụng quy trình xóa sạch, rút lui hoặc bỏ đăng ký theo cách thủ công thiết bị](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Làm thế nào để chỉ xóa dữ liệu công ty từ các ứng dụng được quản lý trên InTune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Xóa tất cả dữ liệu khỏi thiết bị macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).