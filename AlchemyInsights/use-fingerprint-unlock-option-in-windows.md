---
title: Sử dụng tùy chọn mở khóa dấu vân tay trong Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972021"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Sử dụng tùy chọn mở khóa dấu vân tay trong Windows 10

**Bật Tính năng Windows Hello vân tay**

Để mở khóa Windows 10 bằng dấu vân tay của bạn, bạn cần thiết lập dấu Vân tay Windows Hello bằng cách thêm (cho phép Windows học cách nhận dạng) ít nhất một ngón tay. 

1. Đi tới Cài đặt > **khoản người > chọn Đăng nhập (hoặc** bấm vào [đây).](ms-settings:signinoptions?activationSource=GetHelp) Các tùy chọn đăng nhập sẵn có sẽ được liệt kê. Ví dụ:

    ![Tùy chọn đăng nhập.](media/sign-in-options.png)

2. Bấm hoặc nhấn vào **Windows Hello Vân tay**, sau đó bấm Thiết **lập**. Trong cửa sổ Windows Hello lập, bấm **vào Bắt đầu**. Cảm biến dấu vân tay sẽ kích hoạt và bạn sẽ được yêu cầu đặt ngón tay lên cảm biến:

   ![Cảm biến dấu vân tay.](media/fingerprint-sensor.png)

3. Làm theo các hướng dẫn, điều này sẽ yêu cầu bạn quét ngón tay nhiều lần. Khi quá trình này hoàn tất, bạn sẽ có tùy chọn thêm các ngón tay khác mà bạn có thể muốn sử dụng để đăng nhập. Lần sau khi bạn đăng nhập vào Windows 10, bạn sẽ có tùy chọn sử dụng dấu vân tay của mình để đăng nhập.

**Windows Hello Dấu vân tay không có sẵn dưới dạng tùy chọn đăng nhập**

Nếu Windows Hello Dấu vân tay không hiển thị dưới dạng tùy chọn trong tùy chọn Đăng nhập **,** điều đó có nghĩa là Windows không biết bất kỳ đầu đọc dấu vân tay/máy quét nào được gắn với PC của bạn hoặc chính sách hệ thống ngăn chặn việc sử dụng PC của bạn (nếu ví dụ như PC của bạn được quản lý bởi nơi làm việc của bạn). Để khắc phục sự cố: 

1. Chọn nút **Bắt đầu** trong Thanh tác vụ và tìm kiếm Trình quản lý **Thiết bị**.

2. Bấm hoặc nhấn để mở Trình **quản lý Thiết bị**.

3. Trong Trình quản lý Thiết bị, mở rộng thiết bị Sinh trắc bằng cách bấm vào hình V của thiết bị.

   ![Thiết bị sinh trắc.](media/biometric-devices.png)

4. Máy quét dấu vân tay của bạn phải được liệt kê dưới dạng thiết bị sinh trắc, chẳng hạn như máy quét Synaptics WBDI:

   ![Thiết bị sinh trắc.](media/biometric-devices-expanded.png)

5. Nếu máy quét dấu vân tay của bạn không hiển thị và máy quét được tích hợp vào PC của bạn, hãy truy cập trang web của nhà sản xuất PC. Trong phần hỗ trợ kỹ thuật cho mô hình PC của bạn, hãy tìm kiếm trình điều Windows 10 máy quét mà bạn có thể cài đặt.

6. Nếu máy quét tách biệt với PC (gắn với USB), hãy truy nhập trang web của nhà sản xuất máy quét để tìm và cài đặt phần mềm trình điều khiển thiết bị Windows 10 của kiểu máy quét bạn có.
