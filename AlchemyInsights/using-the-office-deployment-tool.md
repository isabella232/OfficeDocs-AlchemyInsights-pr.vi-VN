---
title: Sử dụng công cụ triển khai Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794933"
---
# <a name="using-the-office-deployment-tool-odt"></a>Sử dụng công cụ triển khai Office (ODT)

Bạn sử dụng công cụ triển khai Office (ODT) để triển khai các phiên bản Office 365 của Office. Công cụ triển khai Office (setup.exe) được chạy từ dòng lệnh và sử dụng một tệp XML cấu hình để xác định thiết đặt nào cần áp dụng khi triển khai Office.
  
1. Tải xuống phiên bản mới nhất của công cụ triển khai Office từ [Trung tâm tải xuống của Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Sử dụng [công cụ tùy chỉnh Office (tháng mười)](https://config.office.com) để chọn tùy chọn triển khai của bạn và tạo tệp XML cấu hình. Xuất tệp cấu hình và đặt nó cục bộ trên cùng một thư mục mà setup.exe cư trú.

    **Lưu ý:** Các sự cố về cài đặt Office thường xảy ra do các tệp cấu hình cấu hình sai hoặc định dạng. Để tránh các vấn đề như vậy, chúng tôi khuyên bạn nên sử dụng công cụ tùy chỉnh Office để tạo tệp cấu hình. Bạn cũng có thể nhập các tệp cấu hình hiện có vào công cụ tùy chỉnh Office.

3. Từ dấu nhắc lệnh nâng cao, hãy chuyển đến vị trí nơi setup.exe cư trú và chạy công cụ triển khai Office trong chế độ tải xuống và xác định tệp cấu hình bạn vừa lưu. Trong ví dụ này, tệp cấu hình được đặt tên là Configuration.xml:

```setup.exe /download Configuration.xml```

4. chạy công cụ triển khai Office trong chế độ cấu hình và xác định tệp cấu hình.

```setup.exe /configure Configuration.xml```

**Lưu ý:** Bạn phải chạy bước này từ máy tính khách mà bạn muốn cài đặt Office và bạn phải có quyền quản trị cục bộ trên máy tính đó.

Để tìm hiểu thêm về cách sử dụng công cụ triển khai Office cho các tình huống triển khai ứng dụng Microsoft 365 cho doanh nghiệp của bạn, hãy xem [tổng quan về công cụ triển khai Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Để biết thêm chi tiết về cách sử dụng công cụ tùy chỉnh Office, hãy xem [tổng quan về công cụ tùy chỉnh Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
