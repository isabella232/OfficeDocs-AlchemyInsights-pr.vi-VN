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
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085854"
---
# <a name="using-the-office-deployment-tool-odt"></a>Sử dụng công cụ triển khai Office (ODT)

Bạn sử dụng công cụ triển khai Office (ODT) để triển khai các phiên bản Office 365 của Office. Công cụ triển khai Office (setupodt.exe) được chạy từ dòng lệnh và sử dụng một tệp XML cấu hình để xác định thiết đặt nào cần áp dụng khi triển khai Office.
  
1. Tải xuống phiên bản mới nhất của công cụ triển khai Office từ [Trung tâm tải xuống của Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Sử dụng [công cụ tùy chỉnh Office (tháng mười)](https://config.office.com) để chọn tùy chọn triển khai của bạn và tạo tệp XML cấu hình. Xuất tệp cấu hình và đặt nó cục bộ trên cùng một thư mục mà setupodt.exe cư trú.

    **Lưu ý:** Các sự cố về cài đặt Office thường xảy ra do các tệp cấu hình cấu hình sai hoặc định dạng. Để tránh các vấn đề như vậy, chúng tôi khuyên bạn nên sử dụng công cụ tùy chỉnh Office để tạo tệp cấu hình. Bạn cũng có thể nhập các tệp cấu hình hiện có vào công cụ tùy chỉnh Office.

3. Từ dấu nhắc lệnh nâng cao, hãy chuyển đến vị trí nơi setupodt.exe cư trú và chạy công cụ triển khai Office trong chế độ tải xuống và xác định tệp cấu hình bạn vừa lưu. Trong ví dụ này, tệp cấu hình được đặt tên là Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. chạy công cụ triển khai Office trong chế độ cấu hình và xác định tệp cấu hình.

```setupodt.exe /configure Configuration.xml```

**Lưu ý:** Bạn phải chạy bước này từ máy tính khách mà bạn muốn cài đặt Office và bạn phải có quyền quản trị cục bộ trên máy tính đó.

Để tìm hiểu thêm về cách sử dụng công cụ triển khai Office cho các tình huống triển khai ứng dụng Microsoft 365 cho doanh nghiệp của bạn, hãy xem [tổng quan về công cụ triển khai Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Để biết thêm chi tiết về cách sử dụng công cụ tùy chỉnh Office, hãy xem [tổng quan về công cụ tùy chỉnh Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
