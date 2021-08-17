---
title: tương tự như tên tệp là tốt nhất
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312847"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Required Alchemy Header H1, H2's don's work." (Đầu trang Alchemy Bắt buộc H1, H2 không hoạt động).
Cách thực hành và hướng dẫn tốt nhất cho việc tạo Alchemy:

1. **Không lồng Alchemy Insights trong thư mục**- điều này sẽ phá vỡ cấu trúc url. Chúng tôi đang tìm cách khắc phục sự cố này.
1. Các tệp trong **thư mục AlchemyInsights** phải có tên tệp chữ thường với gạch nối cho dấu cách ví dụ. **_how-to-enable-litigation-hold_**.
    1. Đưa ID Quy tắc hoặc ID bộ chứa vào cổng [thông tin Đối tác Alchemy](https://alchemyportal.azurewebsites.net) trong trường ms.custom. ví dụ. ***ms.custom: 100021***
1. Sử dụng phần còn lại của siêu dữ liệu ở phía trên cùng của tệp này làm mẫu của bạn.
1. Trong cổng thông tin Đối tác [Alchemy,](https://alchemyportal.azurewebsites.net)dẫn hướng xuống mục Tiêu đề Thông tin chuyên sâu cho Khách **hàng:** và sử dụng tiêu đề đó làm điểm bắt đầu cho tiêu đề H1 của bạn cho thông tin chuyên sâu. 

**Ghi** chú : Alchemy Insights PHẢI chỉ có một H1 duy nhất ở trên cùng hoặc sẽ phá vỡ trong quá trình sản xuất. H2 không kết xuất vì vậy hãy dùng chữ **đậm hoặc** các quy ước khác để biểu thị các phần riêng biệt.
1. Tiếp theo, điền vào thân văn bản bằng cách sử dụng tài liệu nháp Customer Insights của trang Quy tắc Alchemy
    1. Danh sách dấu đầu dòng hoàn toàn không sao
    1. Danh sách đánh số nữa
    1. **In** *đậm và in* đậm là kiểu ok
    1. Liên kết luôn phải là **"liên kết đến web"/liên kết sâu** HOẶC bên ngoài đến các thành phần **UI, chứ không** phải là liên kết nội bộ.
    1. Ảnh không được hỗ trợ chính thức vào thời điểm này nhưng ảnh đã có trong lộ trình.

Và điều này thực sự đã có một chút thời gian quá dài. Cách thực hành tốt nhất là khoảng 400 ký tự ---------------------------------

Sau khi nội dung của bạn đã sẵn sàng, hãy kéo nội dung đó vào nhánh trực tiếp. Sau đó, đi đến [cổng thông tin Đối tác Alchemy](https://alchemyportal.azurewebsites.net) và nhập tên tệp vào trường url. 