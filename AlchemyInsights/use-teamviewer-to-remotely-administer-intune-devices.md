---
title: Sử dụng TeamViewer để quản lý từ xa các thiết bị InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555755"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Sử dụng TeamViewer để quản lý từ xa các thiết bị InTune

Thiết bị được quản lý bởi InTune có thể được dùng từ xa bằng cách sử dụng [TeamViewer](https://www.teamviewer.com/).

Quản lý InTune bằng cách sử dụng TeamViewer, sử dụng các bước sau: 

Bắt đầu bằng cách lấy thông tin từ TeamViewer để thiết lập kết nối TeamViewer trên InTune. Điều này cho phép quản trị viên nhập thông tin đăng nhập trong giao diện người dùng TeamViewer Connector trong thiết bị, thao tác một lần để thiết lập liên kết giữa InTune và dịch vụ TeamViewer.

**Phần 1: bắt đầu một phiên với một thiết bị từ xa**

1. Trong **tất cả các thiết bị**, chọn thiết bị bạn muốn bắt đầu một phiên làm việc từ xa.
2. Từ **... Hơn nữa**, chọn **phiên hỗ trợ từ xa mới**.
3. Chọn **có** để thừa nhận bạn muốn thiết lập một phiên làm từ xa.
    Sau khi yêu cầu "bắt đầu phiên làm việc từ xa mới" được công nhận bởi dịch vụ TeamViewer, bạn sẽ thấy một tùy chọn để **khởi động hỗ trợ từ xa** theo chi tiết của ngăn tổng quan (hoặc, Essentials) cho thiết bị. Chọn **xem thêm** để mở rộng ngăn và hiển thị trạng thái hỗ trợ từ xa.
4. Chọn **khởi động phiên từ xa** để bắt đầu phiên ở phía quản trị.
5. Chọn để tải về các nhị phân TeamViewer (Windows), và chọn **Run**.<br/>
    **Lưu ý** Bạn có thể bỏ qua bất kỳ trang trình duyệt web nào được mở vào trang web TeamViewer.

6. Thừa nhận yêu cầu cho ứng dụng TeamViewer để thực hiện thay đổi trên thiết bị (chỉ dành cho Windows).
7. Ứng dụng TeamViewer khởi động và bao gồm mã phiên để xác thực kết nối với thiết bị từ xa.

**Phần 2: trên thiết bị đang được nhắm mục tiêu cho một phiên làm việc từ xa**

1. Mở cổng công ty InTune.
2. Tìm cờ thông báo: "người quản trị CNTT của bạn đang yêu cầu quyền kiểm soát thiết bị này cho phiên hỗ trợ từ xa" và chọn thông báo.
3. Chọn để tải xuống ứng dụng TeamViewer hoặc xác nhận tải xuống ứng dụng TeamViewer từ cửa hàng ứng dụng và chọn **chạy**.
    **Lưu ý** Bạn có thể bỏ qua bất kỳ trang trình duyệt web nào được mở vào trang web TeamViewer.

4. Thừa nhận yêu cầu cho ứng dụng TeamViewer để thực hiện thay đổi trên thiết bị (chỉ dành cho Windows).
5. Ứng dụng TeamViewer khởi động và bao gồm mã phiên để xác thực kết nối với thiết bị từ xa.
6. Một popup sẽ hỏi nếu bạn muốn cho phép phiên để bắt đầu.

**Lưu ý** Mã phiên được tạo bởi dịch vụ TeamViewer chỉ sử dụng một lần. Nếu bạn bị mất kết nối, bạn phải:

1. Đóng phiên bản ứng dụng TeamViewer trên thiết bị từ xa và trên trạm làm việc quản trị.
2. Đóng cổng công ty trên thiết bị từ xa.
3. Khởi tạo mới "phiên hỗ trợ từ xa mới" từ cổng quản trị.
4. Mở lại cổng công ty trên thiết bị từ xa để nhận được thông báo mới.
5. Tải xuống và mở ứng dụng TeamViewer trên cả thiết bị từ xa và máy trạm quản trị, như trước đây.