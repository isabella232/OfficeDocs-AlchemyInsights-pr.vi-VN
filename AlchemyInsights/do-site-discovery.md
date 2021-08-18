---
title: Thực hiện khám phá site
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
ms.openlocfilehash: 5ae99192c769dd5d5acae1c6e8f9b021e824b465
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322189"
---
# <a name="do-site-discovery"></a>Thực hiện khám phá site

Nếu tổ chức của bạn vẫn sử dụng các ứng dụng web thừa tự và các gói để sử dụng chế độ Internet Explorer (mà hầu hết khách hàng làm), bạn nên thực hiện một số khám phá site bổ sung.

**Bạn đã triển khai một phiên bản cũ hơn của Microsoft Edge**

Nếu bạn đã cấu hình Danh sách Site Doanh nghiệp để làm việc cho phiên bản kế thừa của Microsoft Edge, khi đó việc khám phá site của bạn gần như hoàn thành. Một điều bạn có thể cần làm là thêm các site trung lập.

Site trung lập thường là các site cung cấp tính năng đăng nhập đơn (SSO). Nếu bạn đi đến site trung lập từ Microsoft Edge, bạn muốn ở lại để Microsoft Edge thực. Nếu bạn đi đến một site trung lập ở chế độ Internet Explorer, khi đó bạn muốn duy trì ở chế độ Internet Explorer để xác thực.

Xác định mọi SSO hoặc site trung lập khác mà bạn sử dụng và thêm những site này vào Danh sách Site Doanh nghiệp của bạn.

**Internet Explorer là trình duyệt mặc định của bạn**

Nếu bạn hiện chỉ đang sử dụng Internet Explorer, bạn có thể không biết site nào đã được nâng cấp lên tiêu chuẩn web hiện đại và site nào vẫn cần có Internet Explorer. Bạn sẽ muốn tìm và thêm những site này vào Danh sách Site Doanh nghiệp để bạn chỉ có thể sử dụng chế độ Internet Explorer cho những site đó.

**Lưu** ý: [Khám phá Site Doanh](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) nghiệp phát hiện các site có thể cần chế độ Internet Explorer. Trình duyệt có thể thu thập dữ liệu trên máy tính chạy Windows Internet Explorer 8 đến Internet Explorer 11 trên Windows 10, Windows 8.1 hoặc Windows 7.

**Phân tích dữ liệu**

Sau khi bạn đã thu thập dữ liệu site, chúng tôi đề xuất quy trình bốn bước sau đây để phân tích dữ liệu:
1. Sắp xếp dữ liệu theo miền, rồi theo URL.
2. Xác định ranh giới của ứng dụng để cấu hình cho chế độ Internet Explorer. Bạn muốn bao gồm tất cả các site và điều khiển web xác định ứng dụng, nhưng bạn không muốn bao gồm các site và điều khiển bổ sung. Một số site có thể đơn giản như trong *https://contoso.com/app1* khi những site khác có thể yêu cầu bạn xác định nhiều site và trang.
3. Kiểm tra ứng dụng để xác nhận rằng ứng dụng này hiện không hoạt động. Nhiều site sẽ cung cấp nội dung hiện đại khi chúng phát hiện trình duyệt hiện đại và chỉ cung cấp nội dung kế thừa khi chúng phát hiện Internet Explorer.
4. Thêm ứng dụng vào Danh sách Site Doanh nghiệp nếu nó không kiểm tra được.

**Lưu** ý: Cách thực hành tốt nhất là nhóm tất cả các site thành phần ứng dụng. Bằng cách này, khi bạn nâng cấp một ứng dụng, sẽ dễ dàng hơn để loại bỏ toàn bộ site khỏi chế độ Internet Explorer và bắt đầu sử dụng một trình duyệt hiện đại cho ứng dụng đó.

Sau khi khám phá site xong và đã phân tích dữ liệu, bạn đã sẵn sàng bắt đầu xem chiến lược kênh của mình.

