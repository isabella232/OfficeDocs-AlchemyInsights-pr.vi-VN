---
title: Thay đổi miền yammer mặc định
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 099feb5c58a2b1068a2ec501ff966c6ac73d804d
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991333"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Thay đổi miền yammer mặc định/chính

Yammer URL chứa tên miền chính hiện tại cho mạng yammer của bạn. Tên miền này có thể không khớp với tên miền chính trong Office 365 hoặc Azure AD. Có sự khác biệt về hành vi dựa trên số miền tuỳ chỉnh được thêm vào đối tượng thuê và liệu yammer có cấu hình được hỗ trợ (1 người thuê: 1 mạng hoặc 1:1). Tài liệu về [miền yammer và Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) có sẵn.

Lý do phổ biến nhất mà bạn thấy một tên miền không chính xác là nhiều yammer mạng tồn tại và cần phải được hợp nhất. [Củng cố xuống một mạng duy nhất](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) bằng cách sử dụng công cụ di chuyển mạng là một bước quan trọng đầu tiên. Hoàn thành điều này trước khi cố gắng đặt tên miền chính của bạn.

**Không có miền tùy chỉnh**

Đối với người thuê nhà mới, tên miền mặc định (ví dụ: fabrikam.onmicrosoft.com) từ đối tượng thuê sẽ được sử dụng cho yammer. Tên miền chính được đặt thành yammer.com/fabrikam.onmicrosoft.com.

**Miền tùy chỉnh duy nhất**

Yammer sẽ tự động chọn miền tùy chỉnh (ví dụ: fabrikam.com) từ đối tượng thuê làm miền chính trong yammer. Nó được thiết lập để yammer.com/fabrikam.com. Thay đổi này được thực hiện bởi dịch vụ đồng bộ hoá miền và có thể mất đến 24 giờ để có hiệu lực.

**Nhiều miền tùy chỉnh**

Yammer có thể có một tên miền chính khác với miền thuê mặc định. Vì có nhiều miền tuỳ chỉnh, yammer không cố gắng đoán tên miền chính xác từ những người có sẵn. Bạn cần phải mở một trường hợp hỗ trợ để yêu cầu tên miền chính được thay đổi thành tên miền chính mà bạn chọn.

**Thông tin khắc phục sự cố bổ sung**

Trong một số trường hợp tên miền có thể đã được di chuyển giữa các thuê và dịch vụ đồng bộ hoá miền đã không thể chạy thành công. Bạn có thể gặp phải đăng nhập hoặc các vấn đề khác, ngoài miền chính không chính xác. Để giải quyết vấn đề này, tên miền có thể cần phải được di chuyển đến mạng đúng với sự trợ giúp từ Microsoft support. Tình trạng này yêu cầu hỗ trợ trực tiếp và có thể mất một thời gian để giải quyết, đặc biệt là nếu có một danh sách rất dài các tên miền. Mở một trường hợp hỗ trợ để nhận trợ giúp giải quyết các loại vấn đề này.

Khi làm việc với một nhân viên hỗ trợ, họ sẽ kiểm tra xem các miền được xác minh trên một đối tượng thuê dưới sự kiểm soát của bạn. Họ có thể hỏi các câu hỏi xác minh bổ sung về miền của bạn nếu chúng được thêm vào đối tượng thuê của bạn nhưng không được xác minh bằng DNS. Hãy đảm bảo rằng các miền được xác minh bằng DNS để tăng tốc quá trình.
