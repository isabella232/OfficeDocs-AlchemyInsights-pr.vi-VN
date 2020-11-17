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
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086178"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="69337-102">Các câu hỏi về cách sử dụng công cụ triển khai Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="69337-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="69337-103">Tải xuống công cụ triển khai Office từ [Trung tâm tải xuống của Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="69337-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="69337-104">Sau khi tải xuống tệp, hãy chạy tệp thực thi tự giải nén, trong đó có chứa công cụ thực thi triển khai Office (setupodt.exe) và một tệp cấu hình mẫu (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="69337-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setupodt.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="69337-105">**Để loại trừ hoặc loại bỏ các ứng dụng Microsoft 365 cho các sản phẩm doanh nghiệp từ máy tính khách:**</span><span class="sxs-lookup"><span data-stu-id="69337-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="69337-106">Khi cài đặt ứng dụng Microsoft 365 cho doanh nghiệp, bạn có thể loại trừ các sản phẩm cụ thể.</span><span class="sxs-lookup"><span data-stu-id="69337-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="69337-107">Để thực hiện việc này, hãy làm theo các bước để cài đặt Office bằng ODT, nhưng bao gồm phần tử ExcludeApp trong tệp cấu hình của bạn.</span><span class="sxs-lookup"><span data-stu-id="69337-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="69337-108">Ví dụ, tệp cấu hình này cài đặt tất cả các ứng dụng Microsoft 365 dành cho các sản phẩm doanh nghiệp ngoại trừ Publisher:</span><span class="sxs-lookup"><span data-stu-id="69337-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="69337-109">Tổng quan về công cụ triển khai Office</span><span class="sxs-lookup"><span data-stu-id="69337-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

