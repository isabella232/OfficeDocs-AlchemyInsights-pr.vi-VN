---
title: giống như tên tập tin là tốt nhất
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/15/2019
ms.locfileid: "35800067"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Yêu cầu Alchemy header H1, H2's không làm việc.
Thực tiễn tốt nhất và hướng dẫn cho Alchemy authoring:

1. Không **làm tổ các hiểu biết Alchemy trong thư mục**-điều này sẽ phá vỡ cấu trúc URL. Chúng tôi đang tìm kiếm vào sửa chữa này.
1. Các tệp trong thư mục **AlchemyInsights** nên có tên tập tin chữ thường với dấu gạch ngang cho không gian ex. ***làm thế nào để kích hoạt-tranh chấp giữ***.
    1. Bao gồm ID quy tắc hoặc ID nhóm từ [cổng thông tin đối tác giả kim](https://alchemyportal.azurewebsites.net) trong trường MS. Custom. Ex. ***MS. tùy chỉnh: 100021***
1. Sử dụng phần còn lại của siêu dữ liệu ở đầu tệp này làm mẫu của bạn.
1. Trong [cổng thông tin đối tác giả kim](https://alchemyportal.azurewebsites.net), điều hướng xuống mục **khách hàng Insight tiêu đề:** và sử dụng đó như là một điểm khởi đầu cho tiêu đề H1 của bạn cho cái nhìn sâu sắc. 
    > [!NOTE]
    > Alchemy Insights phải có chỉ có một H1 duy nhất ở đầu hoặc họ sẽ phá vỡ trong sản xuất. H2s không hiển thị hoặc để sử dụng **đậm** hoặc các quy ước khác để biểu thị các phần riêng biệt.
1. Tiếp theo, điền vào nội dung văn bản bằng cách sử dụng tài liệu dự thảo trong phần hiểu biết khách hàng của trang quy tắc giả kim thuật
    1. Danh sách có dấu đầu dòng là tốt
    1. Danh sách số quá
    1. **Bold** và *nghiêng* là một OK
    1. Liên kết phải luôn là **"liên kết đến web"/bên ngoài** hoặc **Deep-liên kết đến các yếu tố giao diện người dùng**, không liên kết nội bộ.
    1. Hình ảnh không được hỗ trợ chính thức vào thời gian này, nhưng nó trên lộ trình.

Và điều này thực sự là đã có một chút quá dài. Thực hành tốt nhất là khoảng 400 ký tự---------------------------------

Sau khi nội dung của bạn đã sẵn sàng, hãy kéo nó đến chi nhánh trực tiếp. Sau đó, đi đến [cổng thông tin đối tác giả kim](https://alchemyportal.azurewebsites.net) và nhập tên tệp vào trường URL. 