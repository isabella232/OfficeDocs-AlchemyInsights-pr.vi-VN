---
title: Cấu hình dịch vụ cung cấp
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
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484049"
---
# <a name="configuring-the-provision-service"></a>Cấu hình dịch vụ cung cấp

Để cung cấp cho người dùng tự động hoạt động, Azure AD yêu cầu chứng danh hợp lệ cho phép nó kết nối với API dịch vụ web ngày làm việc. Ngoài ra, nút kết nối kiểm tra trong ngày làm việc đến ứng dụng cung cấp người dùng quảng cáo cũng xác nhận nếu có thể kết nối với đại diện cung cấp kết nối Azure AD được liên kết với tên miền quảng cáo.

Nếu cổng Azure sẽ trả về lỗi khi lưu chứng danh, hãy làm theo các bước được đề xuất dưới đây:

1. Xác nhận rằng bạn đã cấu hình tài khoản người dùng hệ thống tích hợp workday như đã nêu trong phần hướng dẫn [cấu hình người dùng hệ thống tích hợp trong ngày](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)làm việc.
2. Xác nhận rằng dịch vụ đại diện cung cấp Azure AD kết nối đang được thiết lập và chạy trên Windows Server tại cơ sở của bạn bằng cách sử dụng bảng điều khiển quản lý Dịch vụ. Bạn cũng có thể kiểm tra trạng thái của đại diện trong cổng thông tin Azure bằng cách bấm vào nút xem các đại diện tại chỗ.
3. Đảm bảo rằng bạn đang nhập giá trị cho trường "username Day Username" bằng cách dùng định dạng username@workday-đối tượng thuê. Nếu thiếu tên đối tượng thuê ngày làm việc, xác thực ngày làm việc không thành công.
4. Nếu bạn đang cấu hình tích hợp với đối tượng thuê thực thi ngày làm việc, hãy lưu ý những giờ thời gian ngừng hoạt động của đối tượng thuê ngày làm việc của bạn. Ngày làm việc đã lên lịch đã lên lịch cho người thuê thực thi của mình qua các ngày cuối tuần (thường là từ tối thứ sáu đến buổi sáng thứ bảy) và lỗi kết nối trong cửa sổ downtime này là một vấn đề đã biết tự động giải quyết ngay khi các thuê bao triển khai đang trở lại trực tuyến.
5. Trong các trường hợp hiếm, bạn cũng có thể thấy lỗi này nếu mật khẩu của người dùng hệ thống tích hợp đã thay đổi do làm mới của đối tượng thuê hoặc nếu tài khoản trong trạng thái bị khóa hoặc đã hết hạn. Vui lòng kiểm tra trạng thái của người dùng hệ thống tích hợp với người quản trị ngày làm việc của bạn.

Để biết thêm chi tiết về cách đặt cấu hình ngày làm việc cho tính năng cung cấp tự động, hãy xem [hướng dẫn: cấu hình ngày làm việc cho người dùng tự động cung](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)cấp.
