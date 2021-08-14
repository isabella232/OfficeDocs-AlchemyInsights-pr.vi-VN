---
title: Sử dụng TeamViewer để quản lý các thiết bị Intune từ xa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 35c82f8b91a4a0a75f8aa376771a20e6684620c55e8a06abe59db22cab945139
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53990549"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Sử dụng TeamViewer để quản lý các thiết bị Intune từ xa

Thiết bị do Intune quản lý có thể được quản lý từ xa bằng cách sử [dụng TeamViewer.](https://www.teamviewer.com/)

Để quản trị Intune bằng cách sử dụng TeamViewer, hãy sử dụng các bước sau: 

Bắt đầu bằng việc nhận thông tin xác thực từ TeamViewer để thiết lập Trình kết nối TeamViewer trên Intune. Điều này cho phép người quản trị nhập thông tin xác thực vào UI Trình kết nối TeamViewer bên dưới Thiết bị, thao tác một lần để thiết lập liên kết giữa Intune và dịch vụ TeamViewer.

**Phần 1: Bắt đầu phiên với thiết bị từ xa**

1. Trong **Tất cả thiết** bị, chọn thiết bị mà bạn muốn bắt đầu phiên làm việc từ xa.
2. Từ  **... Thêm,** chọn **Phiên hỗ trợ từ xa mới**.
3. Chọn **Có để** xác nhận bạn muốn thiết lập phiên làm việc từ xa.
    Sau khi yêu cầu "Khởi tạo phiên làm việc từ xa mới" được dịch  vụ TeamViewer chấp nhận, bạn sẽ thấy tùy chọn Bắt đầu trợ giúp từ xa dưới chi tiết của ngăn Tổng quan (hoặc Essentials) dành cho thiết bị. Chọn **Xem Thêm để** bung rộng ngăn và hiện trạng thái Trợ giúp Từ xa.
4. Chọn **Bắt đầu phiên từ** xa để khởi tạo phiên ở phía quản trị viên.
5. Chọn để tải xuống nhị phân TeamViewer (Windows), rồi chọn **Chạy**.<br/>
    **Lưu ý** Bạn có thể bỏ qua bất kỳ trang trình duyệt web nào được mở đến website TeamViewer.

6. Xác nhận yêu cầu ứng dụng TeamViewer thực hiện thay đổi trên thiết bị (chỉ Windows bạn).
7. Ứng dụng TeamViewer khởi động và bao gồm mã phiên để xác thực kết nối với thiết bị từ xa.

**Phần 2: Trên thiết bị đang được hướng mục tiêu cho một phiên làm việc từ xa**

1. Mở cổng thông tin công ty Intune.
2. Tìm cờ thông báo: "Người quản trị CNTT của bạn đang yêu cầu quyền điều khiển thiết bị này cho một phiên hỗ trợ từ xa", và chọn thông báo.
3. Chọn để tải xuống ứng dụng TeamViewer hoặc xác nhận tải xuống ứng dụng TeamViewer từ cửa hàng ứng dụng, rồi chọn **Chạy**.
    **Lưu ý** Bạn có thể bỏ qua bất kỳ trang trình duyệt web nào được mở đến website TeamViewer.

4. Xác nhận yêu cầu ứng dụng TeamViewer thực hiện thay đổi trên thiết bị (chỉ Windows bạn).
5. Ứng dụng TeamViewer khởi động và bao gồm mã phiên để xác thực kết nối với thiết bị từ xa.
6. Cửa sổ bật lên sẽ hỏi liệu bạn có muốn cho phép bắt đầu phiên này không.

**Lưu ý** Mã phiên do dịch vụ TeamViewer tạo chỉ sử dụng một lần. Nếu bạn mất kết nối, bạn phải:

1. Đóng phiên bản của ứng dụng TeamViewer trên thiết bị từ xa và trên máy trạm quản trị.
2. Đóng cổng thông tin công ty trên thiết bị từ xa.
3. Khởi tạo "Phiên Trợ giúp từ xa mới" mới từ cổng thông tin quản trị.
4. Mở lại cổng thông tin công ty trên thiết bị từ xa để nhận thông báo mới.
5. Tải xuống và mở ứng dụng TeamViewer trên cả thiết bị từ xa và máy trạm quản trị, như trước đây.