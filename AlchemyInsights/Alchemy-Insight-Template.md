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
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664156"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"H1 tiêu đề Alchemy bắt buộc, H2's không hoạt động."
Phương pháp tốt nhất và hướng dẫn cho tác giả Alchemy:

1. Không **làm tổ những cái nhìn giả kim thuật trong thư mục**-điều này sẽ ngắt cấu trúc URL. Chúng tôi đang tìm cách khắc phục sự cố này.
1. Các tệp trong thư mục **Alchemyinsights** cần có tên tệp chữ thường với dấu gạch nối cho các dấu cách cũ. ***làm thế nào để kích hoạt-giữ tranh chấp***.
    1. Đưa vào ID quy tắc hoặc ID Xô từ [cổng thông tin đối tác Alchemy](https://alchemyportal.azurewebsites.net) trong trường MS. Custom. OKB. ***MS. Custom: 100021***
1. Sử dụng phần còn lại của siêu dữ liệu ở phía trên cùng của tệp này làm mẫu của bạn.
1. Trong [cổng thông tin đối tác Alchemy](https://alchemyportal.azurewebsites.net), dẫn hướng xuống đến **tiêu đề của khách hàng phần Insight:** và sử dụng làm điểm bắt đầu cho tiêu đề H1 của bạn cho cái nhìn sâu sắc. 
    > [!NOTE]
    > Những cái nhìn giả kim thuật phải chỉ có một H1 duy nhất ở trên cùng hoặc chúng sẽ ngắt trong sản xuất. H2s không khiến cho việc sử dụng các công ước **đậm** hoặc khác để biểu thị các phần riêng biệt.
1. Tiếp theo, điền vào nội dung văn bản bằng cách sử dụng tài liệu dự thảo trong phần Insights của khách hàng của trang quy tắc Alchemy
    1. Danh sách dấu đầu dòng là tốt
    1. Danh sách đánh số quá
    1. **Đậm** và *nghiêng* là một OK
    1. Liên kết luôn phải là **"nối kết đến web"/bên ngoài** hoặc **liên kết sâu đến các thành phần giao diện người dùng**, không liên kết nội bộ.
    1. Ảnh không được hỗ trợ chính thức vào thời điểm này, nhưng trên lộ trình.

Và điều này thực sự là một chút quá dài. Cách thực hành tốt nhất là giới thiệu về 400---------------------------------

Sau khi nội dung của bạn đã sẵn sàng, hãy kéo nó đến chi nhánh trực tiếp. Sau đó, đi đến [cổng thông tin đối tác giả kim](https://alchemyportal.azurewebsites.net) và nhập tên tệp vào trường URL. 