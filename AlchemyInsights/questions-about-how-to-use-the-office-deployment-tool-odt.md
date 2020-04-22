---
title: Câu hỏi về cách sử dụng công cụ triển khai Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698080"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Câu hỏi về cách sử dụng công cụ triển khai Office (ODT)

Tải xuống công cụ triển khai Office từ [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Sau khi tải xuống tệp, chạy tệp thi hành tự giải nén, chứa công cụ triển khai Office thực thi (Setup. exe) và tệp cấu hình mẫu (configuration. xml).
  
 **Để loại trừ hoặc loại bỏ Microsoft 365 ứng dụng cho các sản phẩm doanh nghiệp từ máy khách:**
  
Khi cài đặt Microsoft 365 Apps dành cho doanh nghiệp, bạn có thể loại trừ các sản phẩm cụ thể. Để làm như vậy, hãy làm theo các bước để cài đặt Office với ODT, nhưng bao gồm phần tử ExcludeApp trong tệp cấu hình của bạn. Ví dụ: tệp cấu hình này cài đặt tất cả các ứng dụng Microsoft 365 cho các sản phẩm doanh nghiệp ngoại trừ nhà xuất bản:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Tổng quan về công cụ triển khai Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

