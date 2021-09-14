---
title: Hộp thư nhận thông tin hạn chế thực thi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/31/2021
ms.locfileid: "59316282"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Hộp thư nhận thông tin hạn chế thực thi

Gần đây, Microsoft bắt đầu thực thi ngưỡng cho mỗi hộp thư là 3600 thư mỗi giờ. Để biết thêm thông tin, hãy [xem Exchange Online hạn .](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits) Microsoft 365 những hộp thư nhận được hơn 3600 thư trong một giờ sẽ được tiết lưu trong 60 phút tiếp theo. 

Ngoài ra, giới hạn chặn thư nhận được từ một người gửi (SRP) từ một người gửi cụ thể sẽ được áp dụng các thư nhận được từ Microsoft 365 một người gửi cụ thể. Nếu một người gửi đơn lẻ gửi quá 33% tổng ngưỡng hoặc 1200 thư trong một giờ cuộn đến một người nhận cụ thể, giới hạn SRP được kích hoạt và hộp thư không còn tiếp nhận thư từ người gửi đó nữa. Lưu ý rằng:

- Giới hạn này là ứng dụng cho các email nhận được từ đối tượng thuê khác, người gửi tại chỗ hoặc người gửi Internet.
- Email chuyển phát tới hộp thư sẽ bị chặn trong 60 phút tiếp theo. 
- Người gửi đến các hộp thư này nhận được báo cáo không chuyển phát (5.2.121 hoặc 5.2.122) cho biết hộp thư đã vượt quá ngưỡng chuyển phát tối đa. Intra-tenant (mail within the same tenant) tiếp tục được chuyển phát.
- Khi giới hạn SRP được áp dụng, hộp thư nhận sẽ tiếp tục chấp nhận thư từ những người gửi khác.

Người quản trị có thể theo dõi hoạt động hộp thư hiện tại bằng cách truy nhập báo cáo mới và thông tin chuyên sâu trong trung tâm quản trị Exchange gọi là "Hộp thư vượt quá giới hạn nhận". Thông tin chuyên sâu chỉ xuất hiện khi một đối tượng thuê có các hộp thư vi phạm, trong khi báo cáo luôn xuất hiện trong bảng điều khiển nhưng trống trừ khi một đối tượng thuê có các hộp thư vi phạm.

Để biết thêm thông tin về giới hạn nhận thông tin chuyên sâu, hãy xem Hộp thư vượt quá giới [hạn nhận thông tin chuyên sâu trong EAC mới.](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)

Để biết thêm thông tin về báo cáo vượt quá giới hạn nhận, hãy xem hộp thư vượt quá báo cáo giới hạn nhận [trong EAC mới](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report).