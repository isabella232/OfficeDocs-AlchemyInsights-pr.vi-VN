---
title: Sử dụng công cụ triển khai Office
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
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085854"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="5c67e-102">Sử dụng công cụ triển khai Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="5c67e-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="5c67e-103">Bạn sử dụng công cụ triển khai Office (ODT) để triển khai các phiên bản Office 365 của Office.</span><span class="sxs-lookup"><span data-stu-id="5c67e-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="5c67e-104">Công cụ triển khai Office (setupodt.exe) được chạy từ dòng lệnh và sử dụng một tệp XML cấu hình để xác định thiết đặt nào cần áp dụng khi triển khai Office.</span><span class="sxs-lookup"><span data-stu-id="5c67e-104">The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="5c67e-105">Tải xuống phiên bản mới nhất của công cụ triển khai Office từ [Trung tâm tải xuống của Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="5c67e-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="5c67e-106">Sử dụng [công cụ tùy chỉnh Office (tháng mười)](https://config.office.com) để chọn tùy chọn triển khai của bạn và tạo tệp XML cấu hình.</span><span class="sxs-lookup"><span data-stu-id="5c67e-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="5c67e-107">Xuất tệp cấu hình và đặt nó cục bộ trên cùng một thư mục mà setupodt.exe cư trú.</span><span class="sxs-lookup"><span data-stu-id="5c67e-107">Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="5c67e-108">**Lưu ý:** Các sự cố về cài đặt Office thường xảy ra do các tệp cấu hình cấu hình sai hoặc định dạng.</span><span class="sxs-lookup"><span data-stu-id="5c67e-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="5c67e-109">Để tránh các vấn đề như vậy, chúng tôi khuyên bạn nên sử dụng công cụ tùy chỉnh Office để tạo tệp cấu hình.</span><span class="sxs-lookup"><span data-stu-id="5c67e-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="5c67e-110">Bạn cũng có thể nhập các tệp cấu hình hiện có vào công cụ tùy chỉnh Office.</span><span class="sxs-lookup"><span data-stu-id="5c67e-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="5c67e-111">Từ dấu nhắc lệnh nâng cao, hãy chuyển đến vị trí nơi setupodt.exe cư trú và chạy công cụ triển khai Office trong chế độ tải xuống và xác định tệp cấu hình bạn vừa lưu.</span><span class="sxs-lookup"><span data-stu-id="5c67e-111">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="5c67e-112">Trong ví dụ này, tệp cấu hình được đặt tên là Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="5c67e-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="5c67e-113">4. chạy công cụ triển khai Office trong chế độ cấu hình và xác định tệp cấu hình.</span><span class="sxs-lookup"><span data-stu-id="5c67e-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="5c67e-114">**Lưu ý:** Bạn phải chạy bước này từ máy tính khách mà bạn muốn cài đặt Office và bạn phải có quyền quản trị cục bộ trên máy tính đó.</span><span class="sxs-lookup"><span data-stu-id="5c67e-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="5c67e-115">Để tìm hiểu thêm về cách sử dụng công cụ triển khai Office cho các tình huống triển khai ứng dụng Microsoft 365 cho doanh nghiệp của bạn, hãy xem [tổng quan về công cụ triển khai Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="5c67e-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="5c67e-116">Để biết thêm chi tiết về cách sử dụng công cụ tùy chỉnh Office, hãy xem [tổng quan về công cụ tùy chỉnh Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="5c67e-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
