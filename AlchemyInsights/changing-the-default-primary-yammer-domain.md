---
title: Thay đổi tên miền yammer mặc định
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 6a7215ef7187e8dc6c834470b4724692b239efd4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818022"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Thay đổi tên miền yammer mặc định/chính

URL yammer chứa tên miền chính hiện tại cho mạng yammer của bạn. Tên miền này có thể không khớp với tên miền chính được đặt trong Office 365 hoặc Azure AD. Có sự khác biệt về hành vi dựa trên số lượng tên miền tùy chỉnh được thêm vào đối tượng thuê và liệu yammer nằm trong cấu hình được hỗ trợ (1 người thuê nhà: 1 mạng hoặc 1:1). Tài liệu hướng dẫn trên các [tên miền yammer và Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) sẵn dùng.

Lý do phổ biến nhất mà bạn nhìn thấy tên miền không chính xác là nhiều mạng yammer tồn tại và cần phải được hợp nhất. [Củng cố xuống một mạng duy nhất](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) bằng cách sử dụng công cụ di chuyển mạng là một bước đầu tiên quan trọng. Hoàn thành điều này trước khi cố gắng đặt tên miền chính của bạn.

**Không có tên miền riêng**

Đối với người thuê mới, tên miền mặc định (ví dụ fabrikam.onmicrosoft.com) từ đối tượng thuê sẽ được sử dụng cho yammer. Tên miền chính được đặt thành yammer.com/fabrikam.onmicrosoft.com.

**Tên miền riêng đơn**

Yammer sẽ tự động chọn tên miền tùy chỉnh (ví dụ fabrikam.com) từ đối tượng thuê như tên miền chính trong yammer. Nó được đặt thành yammer.com/fabrikam.com. Thay đổi này được thực hiện bởi dịch vụ đồng bộ tên miền và có thể mất tới 24 giờ để có hiệu lực.

**Nhiều tên miền riêng**

Yammer có thể có tên miền chính khác với tên miền của đối tượng thuê mặc định. Vì có nhiều tên miền riêng, yammer không tìm cách đoán tên miền chính xác từ những mục này. Bạn cần mở một trường hợp hỗ trợ để yêu cầu tên miền chính được thay đổi thành tên miền chính của lựa chọn.

**Thông tin khắc phục sự cố bổ sung**

Trong một số trường hợp tên miền có thể đã được di chuyển giữa các đối tượng thuê và dịch vụ đồng bộ tên miền chưa thể chạy thành công. Bạn có thể gặp phải sự cố đăng nhập hoặc các vấn đề khác, ngoài tên miền chính không chính xác. Để giải quyết sự cố này, các tên miền có thể cần được di chuyển đến đúng mạng với sự trợ giúp từ Microsoft support. Tình huống này đòi hỏi phải có hỗ trợ trực tiếp và có thể mất một thời gian để giải quyết, đặc biệt là nếu có một danh sách các tên miền rất dài. Mở một trường hợp hỗ trợ để nhận trợ giúp giải quyết các kiểu vấn đề này.

Khi làm việc với một nhân viên hỗ trợ, họ sẽ kiểm tra xem tên miền đó được xác nhận trên một người thuê bên dưới điều khiển của bạn. Họ có thể yêu cầu thêm các câu hỏi xác thực về tên miền của bạn nếu chúng được thêm vào đối tượng thuê của bạn nhưng không được xác nhận bởi DNS. Vui lòng đảm bảo rằng các tên miền được xác nhận bởi DNS để tăng tốc quá trình.
