---
title: Sử dụng tùy chọn mở khóa vân tay trong Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588337"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Sử dụng tùy chọn mở khóa vân tay trong Windows 10

**Kích hoạt Windows Hello Fingerprint**

Để mở khóa Windows 10 bằng vân tay của bạn, bạn cần phải thiết lập Windows Hello Fingerprint bằng cách thêm (cho phép Windows tìm hiểu để nhận dạng) ít nhất một ngón tay. 

1. Đi tới **cài đặt > tài khoản > tùy chọn đăng nhập** (hoặc bấm vào [đây](ms-settings:signinoptions?activationSource=GetHelp)). Các tùy chọn đăng nhập có sẵn sẽ được liệt kê. Ví dụ:

    ![Tùy chọn đăng nhập.](media/sign-in-options.png)

2. Bấm hoặc chạm vào **Windows Hello Fingerprint**, sau đó nhấp vào **thiết lập**. Trong cửa sổ thiết lập Windows hello, hãy nhấp vào bắt **đầu**. Cảm biến vân tay sẽ kích hoạt và bạn sẽ được yêu cầu để ngón tay lên cảm biến:

   ![Cảm biến vân tay.](media/fingerprint-sensor.png)

3. Thực hiện theo các hướng dẫn, sẽ yêu cầu bạn liên tục quét ngón tay của bạn. Khi điều này kết thúc, bạn sẽ có tùy chọn thêm các ngón tay khác mà bạn có thể muốn sử dụng để đăng nhập. Lần tiếp theo bạn đăng nhập vào Windows 10, bạn sẽ có tùy chọn sử dụng vân tay của mình để làm như vậy.

**Windows Hello Fingerprint không khả dụng dưới dạng tùy chọn đăng nhập**

Nếu Windows Hello Fingerprint không được hiển thị dưới dạng tùy chọn trong **tùy chọn đăng nhập**, có nghĩa là Windows không biết bất kỳ trình đọc vân tay/máy quét nào được gắn vào máy tính của bạn hoặc chính sách hệ thống sẽ ngăn việc sử dụng nó (ví dụ: PC của bạn được quản lý bởi công sở của bạn). Để khắc phục sự cố: 

1. Chọn nút **bắt đầu** trong thanh tác vụ và tìm kiếm **trình quản lý thiết bị**.

2. Nhấp hoặc nhấn để mở **trình quản lý thiết bị**.

3. Trong quản lý thiết bị, mở rộng thiết bị sinh trắc học bằng cách nhấp vào Chevron của nó.

   ![Thiết bị sinh trắc học.](media/biometric-devices.png)

4. Máy quét vân tay của bạn sẽ được liệt kê dưới dạng thiết bị sinh trắc học, chẳng hạn như máy quét Synaptics WBDI:

   ![Thiết bị sinh trắc học.](media/biometric-devices-expanded.png)

5. Nếu máy quét vân tay của bạn không được hiển thị và máy quét được tích hợp vào PC của bạn, hãy truy cập trang web của nhà sản xuất PC. Trong phần hỗ trợ kỹ thuật cho mô hình máy tính của bạn, hãy tìm kiếm trình điều khiển Windows 10 cho máy quét mà bạn có thể cài đặt.

6. Nếu máy quét tách biệt với PC (đính kèm qua USB), hãy truy cập trang web của nhà sản xuất máy quét để tìm và cài đặt phần mềm trình điều khiển thiết bị Windows 10 cho mô hình máy quét mà bạn có.
