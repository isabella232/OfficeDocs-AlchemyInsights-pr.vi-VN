---
title: Sử dụng Công cụ Office dụng
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
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083792"
---
# <a name="using-the-office-deployment-tool-odt"></a>Sử dụng Công cụ triển Office Kế hoạch (ODT)

Bạn sử dụng Công cụ Office Dụng cụ Triển khai (ODT) để triển khai và Office 365 bản của Office. Công cụ Triển Office (setup.exe) chạy từ dòng lệnh và sử dụng tệp XML cấu hình để xác định những thiết đặt sẽ áp dụng khi triển khai Office.
  
1. Tải xuống phiên bản mới nhất của Công cụ triển Office từ Trung [tâm Tải xuống của Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Sử dụng Công [cụ Office Chỉnh (OCT) để chọn](https://config.office.com) các tùy chọn triển khai của bạn, rồi tạo tệp XML cấu hình. Xuất tệp cấu hình và đặt cục bộ tệp trên cùng một thư mục chứa tệp setup.exe bạn.

    **Lưu ý:** Office cố cài đặt thường xảy ra do tệp cấu hình bị cấu hình sai hoặc sai định dạng. Để tránh các vấn đề như vậy, chúng tôi khuyên bạn nên sử dụng Office Công cụ Tùy chỉnh để tạo tệp cấu hình. Bạn cũng có thể nhập các tệp cấu hình hiện có vào Công Office Tùy chỉnh.

3. Từ lời nhắc chỉ lệnh mức cao, chuyển đến vị trí setup.exe hiện và chạy Công cụ Triển khai Office ở chế độ tải xuống và chỉ định tệp cấu hình bạn vừa lưu. Trong ví dụ này, tệp cấu hình được đặt Configuration.xml:

```setup.exe /download Configuration.xml```

4.Chạy Công cụ Triển Office ở chế độ cấu hình và chỉ định tệp cấu hình.

```setup.exe /configure Configuration.xml```

**Lưu ý:** Bạn phải chạy bước này từ máy tính khách mà bạn muốn cài đặt Office và bạn phải có quyền người quản trị cục bộ trên máy tính đó.

Để tìm hiểu thêm về cách sử dụng Công cụ Triển khai Office cho các kịch bản triển khai Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn của bạn, hãy xem Tổng quan [về Công cụ Triển khai Office trang](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Để biết thêm chi tiết về cách sử dụng Công cụ Office Chỉnh, hãy xem [Tổng quan về Công cụ Office Tùy chỉnh](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
