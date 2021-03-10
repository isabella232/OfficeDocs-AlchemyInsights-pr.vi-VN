---
title: Thực hiện khám phá trang
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694552"
---
# <a name="do-site-discovery"></a>Thực hiện khám phá trang

Nếu tổ chức của bạn vẫn sử dụng các ứng dụng web kế thừa và các gói sử dụng chế độ Internet Explorer (mà hầu hết khách hàng thực hiện), thì bạn nên thực hiện một số khám phá trang bổ sung.

**Bạn đã triển khai phiên bản Microsoft Edge cũ hơn**

Nếu bạn đã cấu hình danh sách trang web doanh nghiệp của bạn để làm việc cho phiên bản kế thừa của Microsoft Edge, sau đó phát hiện trang web của bạn gần như đã hoàn tất. Một trong những điều bạn có thể cần làm là thêm site trung lập.

Site trung bình thường là các site cung cấp đăng nhập đơn (SSO). Nếu bạn đi đến một site trung lập từ Microsoft Edge, thì bạn muốn ở trong Microsoft Edge để xác thực. Nếu bạn đi đến một site trung lập trong chế độ Internet Explorer, thì bạn muốn giữ lại trong chế độ Internet Explorer để xác thực.

Xác định bất kỳ SSO hoặc các site trung lập nào mà bạn sử dụng và thêm vào danh sách trang web doanh nghiệp của bạn.

**Internet Explorer là trình duyệt mặc định của bạn**

Nếu bạn chỉ đang dùng Internet Explorer, bạn có thể không biết site nào đã nâng cấp lên tiêu chuẩn web hiện đại và vẫn yêu cầu Internet Explorer. Bạn sẽ muốn tìm và thêm các site này vào danh sách site của doanh nghiệp để bạn có thể sử dụng chế độ Internet Explorer cho các site đó.

> [!NOTE]
> [Khám phá trang Enterprise phát hiện](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) ra các site có thể cần chế độ Internet Explorer. Ứng dụng này có thể thu thập dữ liệu trên các máy tính chạy Windows Internet Explorer 8 thông qua Internet Explorer 11 trên Windows 10, Windows 8,1 hoặc Windows 7.

**Phân tích dữ liệu**

Sau khi bạn đã thu thập dữ liệu site, chúng tôi khuyên bạn nên quy trình bốn bước sau đây để phân tích dữ liệu:
1. Sắp xếp dữ liệu theo tên miền, rồi theo URL.
2. Xác định ranh giới của một ứng dụng để cấu hình cho chế độ Internet Explorer. Bạn muốn bao gồm tất cả các site và điều khiển web xác định ứng dụng, nhưng bạn không muốn bao gồm các site và điều khiển bổ sung. Một số site có thể đơn giản như *https://contoso.com/app1* trong khi những người khác có thể yêu cầu bạn xác định nhiều site và trang.
3. Kiểm tra ứng dụng để xác nhận rằng nó không hoạt động chính. Nhiều site sẽ cung cấp nội dung hiện đại khi họ phát hiện ra một trình duyệt hiện đại và chỉ cung cấp nội dung kế thừa khi họ phát hiện Internet Explorer.
4. Thêm ứng dụng vào danh sách site doanh nghiệp của bạn nếu nó không được kiểm tra.

> [!NOTE]
> Thực hành tốt nhất, nhóm tất cả các site có bao gồm một ứng dụng. Bằng cách này, khi bạn nâng cấp một ứng dụng, bạn sẽ dễ dàng loại bỏ toàn bộ site khỏi chế độ Internet Explorer và bắt đầu sử dụng trình duyệt hiện đại cho ứng dụng đó.

Sau khi bạn đã thực hiện xong với khám phá trang và bạn đã phân tích dữ liệu, bạn đã sẵn sàng để bắt đầu xem chiến lược kênh của mình.

