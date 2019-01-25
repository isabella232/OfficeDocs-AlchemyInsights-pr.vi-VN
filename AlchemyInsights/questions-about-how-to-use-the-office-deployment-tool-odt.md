---
title: Các câu hỏi về làm thế nào để sử dụng công cụ triển khai văn phòng (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29497185"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Các câu hỏi về làm thế nào để sử dụng công cụ triển khai văn phòng (ODT)

Tải về công cụ triển khai Office từ [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Sau khi tải về các tập tin, chạy tập tin thực thi tự giải nén chứa các văn phòng triển khai công cụ thực thi (setup.exe) và một tập tin cấu hình mẫu (configuration.xml).
  
 **Để loại trừ hoặc loại bỏ các sản phẩm Office 365 ProPlus từ máy tính khách hàng:**
  
Khi cài đặt Office 365 ProPlus, bạn có thể loại trừ sản phẩm cụ thể. Để làm như vậy, hãy làm theo các bước để cài đặt văn phòng với ODT, nhưng bao gồm các yếu tố ExcludeApp trong tập tin cấu hình của bạn. Ví dụ, tập tin cấu hình này sẽ cài đặt tất cả các sản phẩm Office 365 ProPlus trừ nhà xuất bản:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Tổng quan về công cụ triển khai văn phòng](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

