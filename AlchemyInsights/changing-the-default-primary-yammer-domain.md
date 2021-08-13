---
title: Thay đổi miền mặc Yammer
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
ms.openlocfilehash: dd29f2dc044fe4ee7f50acc6f0ca491d0ceb80bc360534de10d4010230614f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950138"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Thay đổi miền mặc định/Yammer chính

URL Yammer chứa tên miền chính hiện tại cho mạng Yammer bạn. Tên miền này có thể không khớp với tên miền chính được đặt trong Office 365 hoặc Azure AD. Có những khác biệt trong hành vi dựa trên số lượng tên miền riêng được thêm vào đối tượng thuê và liệu Yammer có ở cấu hình được hỗ trợ hay không (1 Đối tượng thuê: 1 Mạng hay 1:1). Có tài [liệu Yammer miền và địa Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) khác.

Lý do phổ biến nhất khiến bạn thấy tên miền không chính xác là vì nhiều Yammer mạng đã tồn tại và cần được hợp nhất. [Hợp nhất thành một mạng duy nhất bằng cách sử](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) dụng công cụ di chuyển mạng là một bước đầu tiên quan trọng. Hoàn thành việc này trước khi tìm cách đặt miền chính của bạn.

**Không có tên miền riêng**

Đối với các đối tượng thuê mới, miền mặc định (ví dụ: fabrikam.onmicrosoft.com) từ đối tượng thuê sẽ được sử dụng để Yammer. Miền chính được đặt thành miền yammer.com/fabrikam.onmicrosoft.com.

**Tên miền riêng đơn**

Yammer sẽ tự động chọn tên miền riêng (ví dụ: fabrikam.com) từ đối tượng thuê làm miền chính trong Yammer. Nó được đặt thành Yammer.com/fabrikam.com. Thay đổi này do dịch vụ đồng bộ miền thực hiện và có thể mất đến 24 giờ để thay đổi có hiệu lực.

**Nhiều tên miền riêng**

Yammer thể có một tên miền chính khác với tên miền của đối tượng thuê mặc định. Vì có nhiều tên miền riêng, Yammer không thể đoán đúng tên miền từ những tên miền sẵn dùng. Bạn cần mở một trường hợp hỗ trợ để yêu cầu tên miền chính được thay đổi thành miền chính theo lựa chọn của bạn.

**Thông tin khắc phục sự cố bổ sung**

Trong một số trường hợp, miền có thể đã được di chuyển giữa các đối tượng thuê và dịch vụ đồng bộ miền vẫn chưa thể chạy thành công. Ngoài tên miền chính không chính, bạn có thể gặp phải sự cố đăng nhập hoặc các sự cố khác. Để giải quyết sự cố này, bạn có thể cần di chuyển miền tới mạng chính xác với sự trợ giúp từ Bộ trợ giúp Của Microsoft. Tình huống này đòi hỏi sự hỗ trợ trực tiếp và có thể mất một chút thời gian để giải quyết, đặc biệt là nếu có một danh sách tên miền rất dài. Mở một trường hợp hỗ trợ để được hỗ trợ giải quyết các loại sự cố này.

Khi làm việc với nhân viên hỗ trợ, họ sẽ kiểm tra để xác minh miền trên đối tượng thuê thuộc quyền kiểm soát của bạn. Họ có thể đặt câu hỏi xác minh bổ sung về tên miền của bạn nếu chúng được thêm vào đối tượng thuê của bạn nhưng không được xác minh bởi DNS. Vui lòng đảm bảo rằng miền được xác minh bằng DNS để tăng tốc quy trình.
