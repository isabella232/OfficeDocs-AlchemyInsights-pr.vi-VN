---
title: Sử dụng TeamViewer để quản lý từ xa các thiết bị InTune
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
ms.openlocfilehash: e931b2092ab049bc01c600344cbd4702848abcd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798470"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Sử dụng TeamViewer để quản lý từ xa các thiết bị InTune

Các thiết bị được quản lý bởi InTune có thể được quản lý từ xa bằng cách sử dụng [TeamViewer](https://www.teamviewer.com/).

Để quản lý InTune bằng cách dùng TeamViewer, hãy sử dụng các bước sau đây: 

Bắt đầu bằng cách thu thập thông tin xác thực từ TeamViewer để thiết lập trình kết nối TeamViewer trên InTune. Điều này cho phép người quản trị nhập chứng danh trong giao diện người dùng trình xem TeamViewer bên dưới thiết bị, thao tác một lần để thiết lập liên kết giữa InTune và dịch vụ TeamViewer.

**Phần 1: bắt đầu một phiên với thiết bị từ xa**

1. Bên dưới **tất cả thiết bị**, chọn thiết bị mà bạn muốn bắt đầu một phiên từ xa.
2. Từ  **... Xem thêm**, chọn **phiên mới hỗ trợ từ xa**.
3. Chọn **có** để xác nhận bạn muốn thiết lập một phiên làm việc từ xa.
    Sau khi "bắt đầu một phiên làm việc từ xa mới" được dịch vụ TeamViewer nhận ra, bạn sẽ thấy một tùy chọn để **khởi động hỗ trợ từ xa** dưới phần chi tiết của Tổng quan (hoặc, Essentials) cho thiết bị. Chọn **xem thêm** để bung rộng ngăn và hiển thị trạng thái hỗ trợ từ xa.
4. Chọn **bắt đầu phiên từ xa** để bắt đầu phiên ở bên quản trị.
5. Chọn tải xuống nhị phân TeamViewer (Windows), rồi chọn **chạy**.<br/>
    **Ghi chú** Bạn có thể bỏ qua bất kỳ trang trình duyệt web nào được mở đến trang web TeamViewer.

6. Xác nhận yêu cầu ứng dụng TeamViewer sẽ thực hiện các thay đổi trên thiết bị (chỉ dành cho Windows).
7. Ứng dụng TeamViewer bắt đầu và bao gồm mã phiên để xác thực kết nối với thiết bị từ xa.

**Phần 2: trên thiết bị đang được nhắm đến phiên làm việc từ xa**

1. Mở cổng thông tin công ty InTune.
2. Tìm cờ thông báo: "người quản trị CNTT của bạn đang yêu cầu điều khiển thiết bị này cho một phiên hỗ trợ từ xa", rồi chọn thông báo.
3. Chọn tải xuống ứng dụng TeamViewer hoặc xác nhận tải xuống ứng dụng TeamViewer từ App Store, rồi chọn **chạy**.
    **Ghi chú** Bạn có thể bỏ qua bất kỳ trang trình duyệt web nào được mở đến trang web TeamViewer.

4. Xác nhận yêu cầu ứng dụng TeamViewer sẽ thực hiện các thay đổi trên thiết bị (chỉ dành cho Windows).
5. Ứng dụng TeamViewer bắt đầu và bao gồm mã phiên để xác thực kết nối với thiết bị từ xa.
6. Bật lên sẽ hỏi bạn có muốn cho phép phiên bắt đầu hay không.

**Ghi chú** Các mã phiên được tạo bởi dịch vụ TeamViewer chỉ được sử dụng một lần. Nếu bạn bị mất kết nối, bạn phải:

1. Đóng phiên bản của ứng dụng TeamViewer trên thiết bị từ xa và trên máy trạm quản trị.
2. Đóng cổng thông tin công ty trên thiết bị từ xa.
3. Khởi tạo một phiên mới "hỗ trợ từ xa mới" từ cổng thông tin quản trị.
4. Mở lại cổng thông tin công ty trên thiết bị từ xa để nhận được thông báo mới.
5. Tải xuống và mở ứng dụng TeamViewer trên cả thiết bị từ xa và máy trạm quản trị, như trước đây.