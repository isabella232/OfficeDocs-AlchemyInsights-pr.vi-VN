---
title: Bằng cách sử dụng công cụ triển khai văn phòng
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28320888"
---
# <a name="using-the-office-deployment-tool-odt"></a>Bằng cách sử dụng công cụ triển khai văn phòng (ODT)

Bạn sử dụng công cụ triển khai văn phòng (ODT) để triển khai Office 365 các phiên bản của Office. Công cụ triển khai văn phòng (setup.exe) chạy từ dòng lệnh và sử dụng một tập tin XML cấu hình để xác định những cài đặt để áp dụng khi triển khai các văn phòng.
  
1. Tải về phiên bản mới nhất của công cụ triển khai Office từ [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
    
2. Sử dụng [Công cụ Tuỳ chỉnh Office (OCT)](https://config.office.com) để chọn các tuỳ chọn triển khai của bạn và tạo ra các tệp tin XML cấu hình. Xuất khẩu các tập tin cấu hình và đặt nó tại địa phương vào cùng một thư mục nơi cư trú của setup.exe. 
    
    **Lưu ý:** Văn phòng cài đặt vấn đề thường xảy ra do sai hoặc tập tin cấu hình malformatted. Để tránh các vấn đề như vậy, chúng tôi khuyên bạn sử dụng công cụ Tuỳ chỉnh Office để tạo tập tin cấu hình. Bạn cũng có thể nhập tập tin cấu hình sẵn có vào công cụ Tuỳ chỉnh Office. 
    
3. Từ một dấu nhắc lệnh nâng lên, chuyển sang vị trí nơi cư trú của setup.exe và chạy công cụ triển khai Office trong chế độ tải về và xác định tập tin cấu hình mà bạn chỉ cần lưu lại. Trong ví dụ này, tập tin cấu hình được đặt tên Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Chạy công cụ triển khai văn phòng trong cấu hình chế độ và chỉ định tập tin cấu hình.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Lưu ý:** Bạn phải chạy bước này từ máy tính khách hàng mà bạn muốn cài đặt văn phòng và bạn phải có quyền quản trị cục bộ trên máy tính đó. 
    
Để tìm hiểu thêm về cách sử dụng công cụ triển khai Office cho các tình huống triển khai Office 365 ProPlus của bạn, hãy xem [tổng quan về công cụ triển khai văn phòng](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Để biết thêm chi tiết về cách sử dụng công cụ Tuỳ chỉnh Office, hãy xem [tổng quan về công cụ Tuỳ chỉnh Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
  

