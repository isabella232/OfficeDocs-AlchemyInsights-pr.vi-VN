---
title: Các câu hỏi về cách sử dụng Công Office Triển khai Máy chủ (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959705"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Các câu hỏi về cách sử dụng Công Office Triển khai Máy chủ (ODT)

Tải xuống Công Office Triển khai Microsoft từ [Trung tâm Tải xuống của Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Sau khi tải xuống tệp, chạy tệp thực thi tự trích xuất, chứa Office Deployment Tool executable (setup.exe) và tệp cấu hình mẫu (configuration.xml).
  
 **Để loại trừ hoặc loại bỏ sản Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn khỏi máy tính khách:**
  
Khi cài đặt Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn, bạn có thể loại trừ các sản phẩm cụ thể. Để thực hiện điều này, hãy làm theo các bước để cài Office với ODT nhưng đưa thành phần ExcludeApp vào tệp cấu hình của bạn. Ví dụ: tệp cấu hình này cài đặt tất cả sản phẩm Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn, ngoại Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Tổng quan về Công cụ Office dụng](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

