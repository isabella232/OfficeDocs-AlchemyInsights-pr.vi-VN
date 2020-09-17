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
ms.openlocfilehash: e0ba83778179abefe3ac4fe3e8ab0303d65ad929
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47804379"
---
# <a name="configure-files-on-demand"></a>Cấu hình các tệp theo yêu cầu

Tệp OneDrive theo yêu cầu sẽ giúp bạn truy nhập tất cả các tệp trong OneDrive mà không cần phải tải xuống tất cả chúng và sử dụng dung lượng lưu trữ trên thiết bị của bạn.

Để cấu hình các tệp theo yêu cầu trên PC của bạn:

1. Chọn biểu tượng đám mây **Onedrive** màu trắng hoặc màu lam trong khu vực thông báo trên thanh tác vụ Windows. Chọn **thiết đặt**> **Trợ giúp & thiết đặt** bánh răng.
2. Trên tab **thiết đặt** , hãy chọn **dung lượng lưu và tải xuống các tệp khi bạn sử dụng** hộp thư.  

Bạn cũng có thể cấu hình các tệp theo yêu cầu bằng cách sử dụng sổ đăng ký.

Nếu bạn vô hiệu hóa thiết đặt này, người dùng Windows 10 có cùng một hành vi đồng bộ với những người dùng của các phiên bản trước của Windows và không thể bật các tệp theo yêu cầu. Nếu bạn không cấu hình thiết đặt này, người dùng có thể bật hoặc tắt các tệp theo yêu cầu.

Cho phép chính sách này đặt giá trị khóa đăng ký sau đây thành 1. Vô hiệu hóa chính sách này đặt giá trị khóa đăng ký sau đây thành 0.

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

Nếu bạn không nhìn thấy tùy chọn tệp theo yêu cầu trong "thiết đặt", hãy đảm bảo rằng "kiểu trình điều khiển bộ lọc tệp của Windows Cloud" được đặt là 2 (AUTO_START). Cho phép tính năng này đặt giá trị khóa đăng ký sau đây thành 2.

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`