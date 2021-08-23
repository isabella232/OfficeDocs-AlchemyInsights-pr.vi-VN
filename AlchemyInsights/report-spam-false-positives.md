---
title: Bạn có muốn báo cáo thư rác bị dương tính với Microsoft không?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396637"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Bạn có thư hợp pháp được đánh dấu là thư rác không?

Thật phiền toái khi email hợp pháp chấm dứt trong thư mục Thư rác hoặc bị cách ly. Hãy cân nhắc những lý do phổ biến nhất về số dương tính giả:

**Ghi đè đối tượng thuê (phổ biến nhất)** Điều này hoàn toàn nằm trong quyền kiểm soát của bạn để khắc phục.

Gửi thông báo trên Bộ bảo vệ Microsoft 365 để phân tích các chính sách và quy tắc tác động; thông tin chi tiết về khả dụng lại sẽ khả dụng trong vòng vài phút.
Xem lại hoặc sửa đổi các chính sách hoặc quy tắc khi áp dụng. 

**Ghi đè Người dùng Cuối (phổ biến)** Điều này hoàn toàn nằm trong quyền kiểm soát của bạn để khắc phục. 

Gửi thông báo trên Bộ bảo vệ Microsoft 365 để phân tích các chính sách và quy tắc tác động; thông tin chi tiết về khả dụng lại sẽ khả dụng trong vòng vài phút. 

Nếu thư bị chặn vì thư được gửi từ địa chỉ trong danh sách Người gửi bị Chặn của người dùng, thì tiêu đề sẽ bao gồm Bản án Lọc Thư rác "SFV:BLK".

**Xác thực email của người gửi** Điều này một phần nằm trong quyền kiểm soát của bạn để khắc phục.

Gửi thư để phân tích các lỗi trong xác thực email của người gửi tại thời điểm chuyển phát; kết quả sẽ khả dụng trong một ngày. 

Nếu bạn sở hữu cơ sở hạ tầng gửi, hãy xem xét cách sắp xếp cơ sở hạ tầng với SPF, DKIM và DMARC để đảm bảo rằng các hệ thống email đích tin cậy thư được gửi từ tên miền của bạn. Ngoài ra, hãy liên hệ với người gửi để giải quyết cấu hình DNS của họ.

**Các dự đoán lọc của Microsoft** Điều này một phần nằm trong quyền kiểm soát của bạn để khắc phục.

Gửi tin nhắn và báo cáo tin nhắn là an toàn; kết quả tìm lại có sẵn trong một ngày. Sử dụng Danh sách Cho phép/Chặn Đối tượng thuê khi bạn không đồng ý với các bản dựng lọc trong những tình huống cụ thể. Tuy nhiên, bạn không nên bỏ qua vĩnh viễn các bản đoán lọc của Microsoft. 

Để biết thêm thông tin, hãy xem:

- Cho phép người dùng cuối của bạn gửi thư đến Microsoft. Microsoft sử dụng các bản gửi này để cải thiện tính hiệu quả của công nghệ bảo vệ email và chúng xuất hiện trong báo cáo gửi đi để bạn có thể sử dụng làm chỉ báo cập nhật chính sách. 

- Để xem video ngắn về việc gửi thư để phân tích, hãy xem [Gửi thư để phân tích](https://go.microsoft.com/fwlink/?linkid=2166435).

- [Sử dụng Gửi Quản trị để gửi các tệp bị nghi là thư rác, lừa đảo qua mạng, URL và tệp đến Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Quản lý Danh sách Cho phép/Chặn của Đối tượng thuê](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Tiêu đề thư chống thư rác trong Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Bảo vệ chống thư rác đi trong EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)