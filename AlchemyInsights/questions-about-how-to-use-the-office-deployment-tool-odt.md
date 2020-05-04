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
ms.openlocfilehash: 4aef42df4dde17d15863fca67e41f0ff23e506dc
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010780"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="13d77-102">Câu hỏi về cách sử dụng công cụ triển khai Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="13d77-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="13d77-103">Tải xuống công cụ triển khai Office từ [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="13d77-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="13d77-104">Sau khi tải xuống tệp, chạy tệp thi hành tự giải nén, chứa công cụ triển khai Office thực thi (Setup. exe) và tệp cấu hình mẫu (configuration. xml).</span><span class="sxs-lookup"><span data-stu-id="13d77-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="13d77-105">**Để loại trừ hoặc loại bỏ Microsoft 365 ứng dụng cho các sản phẩm doanh nghiệp từ máy khách:**</span><span class="sxs-lookup"><span data-stu-id="13d77-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="13d77-106">Khi cài đặt Microsoft 365 Apps dành cho doanh nghiệp, bạn có thể loại trừ các sản phẩm cụ thể.</span><span class="sxs-lookup"><span data-stu-id="13d77-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="13d77-107">Để làm như vậy, hãy làm theo các bước để cài đặt Office với ODT, nhưng bao gồm phần tử ExcludeApp trong tệp cấu hình của bạn.</span><span class="sxs-lookup"><span data-stu-id="13d77-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="13d77-108">Ví dụ: tệp cấu hình này cài đặt tất cả các ứng dụng Microsoft 365 cho các sản phẩm doanh nghiệp ngoại trừ nhà xuất bản:</span><span class="sxs-lookup"><span data-stu-id="13d77-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="13d77-109">Tổng quan về công cụ triển khai Office</span><span class="sxs-lookup"><span data-stu-id="13d77-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

