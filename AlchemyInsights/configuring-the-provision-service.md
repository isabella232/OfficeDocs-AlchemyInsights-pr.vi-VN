---
title: Đặt cấu hình dịch vụ Cung cấp
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033300"
---
# <a name="configuring-the-provision-service"></a>Đặt cấu hình dịch vụ Cung cấp

Để việc cung cấp cho người dùng tự động hoạt động, Azure AD yêu cầu thông tin xác thực hợp lệ cho phép họ kết nối với API Dịch vụ Web Workday. Hơn nữa, nút Kiểm tra Kết nối trong ứng dụng Cung cấp Ngày làm việc đến Người dùng AD cũng xác thực liệu nó có thể kết nối với Tác nhân Cung cấp Azure AD Kết nối được liên kết với Miền AD hay không.

Nếu cổng thông tin Azure trả về lỗi khi lưu thông tin xác thực, hãy làm theo các bước được đề xuất dưới đây:

1. Xác nhận rằng bạn đã cấu hình Tài khoản Người dùng Hệ thống Tích hợp Ngày làm việc như đã nêu trong phần hướng dẫn Cấu hình người dùng [hệ thống tích hợp trong Ngày làm việc](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
2. Xác nhận rằng Dịch vụ Tác nhân Cung cấp Azure AD Kết nối cấp đã được thiết lập và chạy trên máy chủ Windows cơ sở của bạn bằng cách sử dụng Bảng điều khiển Quản lý Dịch vụ. Bạn cũng có thể kiểm tra trạng thái của đại diện trong cổng thông tin Azure bằng cách bấm vào nút Xem đại diện tại chỗ.
3. Đảm bảo rằng bạn đang nhập giá trị cho trường "Tên người dùng ngày làm việc" bằng cách sử dụng định username@workday-tên-đối tượng thuê. Nếu tên làm việc-đối tượng thuê bị thiếu, xác thực Ngày làm việc không thành công.
4. Nếu bạn đang cấu hình tích hợp với đối tượng thuê triển khai Ngày làm việc, hãy lưu ý số giờ nghỉ đã lên lịch cho đối tượng thuê Ngày làm việc của bạn. Workday đã lên lịch thời gian xuống cho các đối tượng thuê triển khai của mình vào cuối tuần (thường là từ buổi tối thứ Sáu đến sáng thứ Bảy) và lỗi kết nối trong cửa sổ thời gian nghỉ này là một vấn đề đã biết, tự động giải quyết ngay khi các đối tượng thuê triển khai trở lại trực tuyến.
5. Trong một số trường hợp hiếm gặp, bạn cũng có thể gặp lỗi này nếu mật khẩu của Người dùng Hệ thống Tích hợp đã thay đổi do làm mới đối tượng thuê hoặc nếu tài khoản đang ở trạng thái khóa hoặc hết hạn. Vui lòng kiểm tra trạng thái của người dùng Hệ thống Tích hợp với người quản trị Ngày làm việc của bạn.

Để biết thêm chi tiết về việc đặt cấu hình ngày làm việc cho việc cung cấp tự động, hãy xem mục Hướng dẫn: Đặt cấu hình Ngày làm việc [để cung cấp tự động cho người dùng.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
