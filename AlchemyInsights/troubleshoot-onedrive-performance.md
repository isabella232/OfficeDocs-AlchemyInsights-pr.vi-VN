---
title: Khắc phục sự cố hiệu suất OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: a78ef48aa92cbcfa27f14aa755e4810e410dddc1
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35367263"
---
# <a name="troubleshoot-onedrive-performance"></a>Khắc phục sự cố hiệu suất OneDrive

Nếu bạn đang gặp phải một chậm hơn so với dự kiến sẽ đồng bộ, hoặc tương tự như các vấn đề hiệu suất với OneDrive:

- Xác nhận không có không có vấn đề bằng cách sử dụng [Bảng điều khiển dịch vụ y tế](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fportal.office.com%2Fadminportal%2Fhome%23%2Fservicehealth&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051385661&sdata=z3OU7adaVjJorTGK8v7Ipo35E5vkk35lVCEzgGYQoNo%3D&reserved=0).

- [Sử Files On Demand](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2Fsave-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051395670&sdata=QN1F4v1q6pNV2hIZ5LCZTtIbuv%2FR7lH5C5g%2FAFJQhrM%3D&reserved=0) do đó bạn có thể truy cập vào tất cả các tập tin trong OneDrive mà không cần phải tải về tất cả chúng và sử dụng không gian lưu trữ trên thiết bị của bạn.

- [Xem xét thực tiễn tốt nhất](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Foffice365%2Fenterprise%2Fnetwork-planning-and-performance&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051405678&sdata=RQCPPj7XPAm4IK6jKf1xugHnxXqqJoKK%2BlEENg7WrDQ%3D&reserved=0) để mạng lập kế hoạch và hiệu suất.

- [Tối đa hoá tải lên và tải về tốc độ](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2FMaximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051405678&sdata=vR4z9GSeObeKY3ouE7oru4Vr%2FGn%2FghUoFBjpRQbfvhA%3D&reserved=0), đặc biệt là nếu bạn đang đồng bộ hoá thiết bị lần đầu tiên.

- Nếu bạn đang đồng bộ hoá một thư viện với hơn 100.000 mặt hàng, đồng bộ OneDrive có vẻ bị mắc kẹt trong một thời gian dài, hoặc tình trạng cho thấy xử lý 0 KB xMB." [Tìm hiểu thêm về đồng bộ hóa tập tin hơn 100.000](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2FInvalid-file-names-and-file-types-in-OneDrive-OneDrive-for-Business-and-SharePoint-64883a5d-228e-48f5-b3d2-eb39e07630fa%23synctoomany&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051415686&sdata=E4zeoBeRBnlGB1haZXTy%2FJfXMBWSPZCbp6JQvt5qX2o%3D&reserved=0) cũng như [của OneDrive được hỗ trợ giới hạn là 300.000 tập tin](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2FInvalid-file-names-and-file-types-in-OneDrive-OneDrive-for-Business-and-SharePoint-64883a5d-228e-48f5-b3d2-eb39e07630fa%23numberitemscanbesynced&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051425695&sdata=uqBKB3ykz9QDOPRmSf5YIKBUiNa57IdQVzeLZWL%2BMWc%3D&reserved=0).

- Khi người dùng vượt quá giới hạn sử dụng, SharePoint Online throttles bất kỳ yêu cầu thêm từ đó tài khoản người dùng trong một thời gian ngắn. Tất cả các hành động của người dùng được throttled trong khi các ga có hiệu lực.
