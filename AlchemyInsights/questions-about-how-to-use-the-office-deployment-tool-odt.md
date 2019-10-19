---
title: Câu hỏi về cách sử dụng công cụ triển khai Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553562"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="730ea-102">Câu hỏi về cách sử dụng công cụ triển khai Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="730ea-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="730ea-103">Tải xuống công cụ triển khai Office từ [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="730ea-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="730ea-104">Sau khi tải xuống tệp, chạy tệp thi hành tự giải nén, chứa công cụ triển khai Office thực thi (Setup. exe) và tệp cấu hình mẫu (configuration. xml).</span><span class="sxs-lookup"><span data-stu-id="730ea-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="730ea-105">**Để loại trừ hoặc loại bỏ các sản phẩm Office 365 ProPlus từ máy khách:**</span><span class="sxs-lookup"><span data-stu-id="730ea-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="730ea-106">Khi cài đặt Office 365 ProPlus, bạn có thể loại trừ các sản phẩm cụ thể.</span><span class="sxs-lookup"><span data-stu-id="730ea-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="730ea-107">Để làm như vậy, hãy làm theo các bước để cài đặt Office với ODT, nhưng bao gồm phần tử ExcludeApp trong tệp cấu hình của bạn.</span><span class="sxs-lookup"><span data-stu-id="730ea-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="730ea-108">Ví dụ, tập tin cấu hình này cài đặt tất cả các sản phẩm Office 365 ProPlus ngoại trừ nhà xuất bản:</span><span class="sxs-lookup"><span data-stu-id="730ea-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="730ea-109">Tổng quan về công cụ triển khai Office</span><span class="sxs-lookup"><span data-stu-id="730ea-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

