---
title: Các tệp theo yêu cầu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 4e3da81ee048c6257e05b998c0f457fa433738fd
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791316"
---
# <a name="configure-files-on-demand"></a>Cấu hình các tệp theo yêu cầu

Các tệp theo yêu cầu của OneDrive yêu cầu [Cập Nhật người tạo mùa thu Windows 10](https://go.microsoft.com/fwlink/p/?linkid=859040) (phiên bản 1709 trở lên) hoặc Windows Server 2019 và OneDrive bản dựng 17.3.7064.1005 trở lên.

Tệp OneDrive theo yêu cầu sẽ giúp bạn truy nhập tất cả các tệp trong OneDrive mà không cần phải tải xuống tất cả chúng và sử dụng dung lượng lưu trữ trên thiết bị của bạn.

Để cấu hình các tệp theo yêu cầu trên PC của bạn:

1. Chọn biểu tượng đám mây **Onedrive** màu trắng hoặc màu lam trong khu vực thông báo trên thanh tác vụ Windows. Chọn **thiết đặt** > **Trợ giúp & thiết đặt** bánh răng.
2. Trên tab **thiết đặt** , hãy chọn **dung lượng lưu và tải xuống các tệp khi bạn sử dụng** hộp thư.  

Bạn cũng có thể cấu hình các tệp theo yêu cầu bằng cách sử dụng sổ đăng ký.

Nếu bạn vô hiệu hóa thiết đặt này, người dùng Windows 10 có cùng một hành vi đồng bộ với những người dùng của các phiên bản trước của Windows và không thể bật các tệp theo yêu cầu. Nếu bạn không cấu hình thiết đặt này, người dùng có thể bật hoặc tắt các tệp theo yêu cầu.

Cho phép chính sách này đặt giá trị khóa đăng ký sau đây thành 1. Vô hiệu hóa chính sách này đặt giá trị khóa đăng ký sau đây thành 0.

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

Nếu bạn không nhìn thấy tùy chọn tệp theo yêu cầu trong "thiết đặt", hãy đảm bảo rằng "kiểu trình điều khiển bộ lọc tệp của Windows Cloud" được đặt là 2 (AUTO_START). Cho phép tính năng này đặt giá trị khóa đăng ký sau đây thành 2.

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`