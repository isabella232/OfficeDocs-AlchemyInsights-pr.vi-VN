---
title: Tệp theo yêu cầu
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
ms.openlocfilehash: 10efdb5e1a90b3e279b8e1716e66a544d0ee34465245f5670930d8a9364a8cc3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53977463"
---
# <a name="configure-files-on-demand"></a>Đặt cấu hình tệp theo yêu cầu

OneDrive Tệp Theo Yêu cầu yêu [cầu Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040) (phiên bản 1709 trở lên) hoặc Windows Server 2019 và OneDrive bản dựng 17.3.7064.1005 trở lên.

OneDrive Tệp theo Yêu cầu giúp bạn truy nhập vào tất cả các tệp trong OneDrive mà không phải tải xuống toàn bộ chúng và sử dụng dung lượng lưu trữ trên thiết bị của bạn.

Để đặt cấu hình Tệp Theo Yêu cầu trên PC của bạn:

1. Chọn biểu tượng đám mây **OneDrive** màu trắng hoặc màu lam trong khu Windows thông báo của thanh tác vụ. Chọn biểu **tượng hình & Cài đặt** hình bánh > **Cài đặt.**
2. Trên tab **Cài đặt,** chọn hộp Lưu **dung lượng và tải xuống tệp khi bạn sử dụng.**  

Bạn cũng có thể đặt cấu hình Tệp Theo Yêu cầu bằng sổ đăng ký.

Nếu bạn tắt thiết đặt này, Windows 10 người dùng sẽ có hành vi đồng bộ giống như người dùng của các phiên bản Windows trước đây và không thể bật tính năng Tệp Theo Yêu cầu. Nếu bạn không cấu hình thiết đặt này, người dùng có thể bật hoặc tắt Tệp Theo Yêu cầu.

Việc bật chính sách này sẽ đặt giá trị khóa đăng ký sau đây là 1. Việc tắt chính sách này sẽ đặt giá trị khóa đăng ký sau đây thành 0.

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

Nếu bạn không thể nhìn thấy tùy chọn Tệp Theo Yêu cầu trong "Cài đặt", hãy đảm bảo rằng loại bắt đầu dịch vụ "Windows Trình điều khiển Bộ lọc Tệp Đám mây" được đặt thành 2 (AUTO_START). Việc bật tính năng này sẽ đặt giá trị khóa đăng ký sau đây là 2.

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`