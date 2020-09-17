---
title: Các câu hỏi về cách sử dụng công cụ triển khai Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774913"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Các câu hỏi về cách sử dụng công cụ triển khai Office (ODT)

Tải xuống công cụ triển khai Office từ [Trung tâm tải xuống của Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Sau khi tải xuống tệp, hãy chạy tệp thực thi tự giải nén, trong đó có chứa công cụ thực thi triển khai Office (setup.exe) và một tệp cấu hình mẫu (configuration.xml).
  
 **Để loại trừ hoặc loại bỏ các ứng dụng Microsoft 365 cho các sản phẩm doanh nghiệp từ máy tính khách:**
  
Khi cài đặt ứng dụng Microsoft 365 cho doanh nghiệp, bạn có thể loại trừ các sản phẩm cụ thể. Để thực hiện việc này, hãy làm theo các bước để cài đặt Office bằng ODT, nhưng bao gồm phần tử ExcludeApp trong tệp cấu hình của bạn. Ví dụ, tệp cấu hình này cài đặt tất cả các ứng dụng Microsoft 365 dành cho các sản phẩm doanh nghiệp ngoại trừ Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Tổng quan về công cụ triển khai Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

