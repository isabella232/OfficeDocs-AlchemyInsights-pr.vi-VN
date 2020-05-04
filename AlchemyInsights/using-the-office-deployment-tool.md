---
title: Sử dụng công cụ triển khai Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010895"
---
# <a name="using-the-office-deployment-tool-odt"></a>Sử dụng công cụ triển khai Office (ODT)

Bạn sử dụng công cụ triển khai Office (ODT) để triển khai Office 365 Phiên bản Office. Công cụ triển khai Office (Setup. exe) chạy từ dòng lệnh và sử dụng tệp XML cấu hình để xác định những cài đặt để áp dụng khi triển khai Office.
  
1. Tải xuống phiên bản mới nhất của công cụ triển khai Office từ [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Sử dụng [công cụ Tuỳ chỉnh Office (Oct)](https://config.office.com) để chọn tuỳ chọn triển khai của bạn và tạo tệp XML cấu hình. Xuất tập tin cấu hình và đặt nó cục bộ trên cùng một thư mục mà Setup. exe cư trú.

    **Lưu ý:** Các vấn đề cài đặt Office thường xảy ra do các tệp cấu hình sai hoặc định dạng lại. Để tránh các vấn đề như vậy, chúng tôi khuyên bạn sử dụng công cụ Tuỳ chỉnh Office để tạo tệp cấu hình. Bạn cũng có thể nhập tệp cấu hình hiện có vào công cụ Tuỳ chỉnh Office.

3. Từ dấu nhắc lệnh nâng cao, chuyển sang vị trí mà Setup. exe cư trú và chạy công cụ triển khai Office trong chế độ tải xuống và chỉ định tệp cấu hình bạn vừa lưu. Trong ví dụ này, tệp cấu hình được đặt tên configuration. xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Chạy công cụ triển khai Office trong chế độ cấu hình và chỉ định tệp cấu hình.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Lưu ý:** Bạn phải chạy bước này từ máy khách mà bạn muốn cài đặt Office và bạn phải có quyền quản trị viên cục bộ trên máy tính.

Để tìm hiểu thêm về cách sử dụng công cụ triển khai Office cho Microsoft 365 ứng dụng cho các trường hợp triển khai doanh nghiệp, hãy xem [tổng quan về công cụ triển khai Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Để biết thêm chi tiết về cách sử dụng công cụ Tuỳ chỉnh Office, hãy xem [tổng quan về công cụ Tuỳ chỉnh Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
