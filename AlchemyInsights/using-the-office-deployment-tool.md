---
title: Sử dụng công cụ triển khai Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726270"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="545a8-102">Sử dụng công cụ triển khai Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="545a8-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="545a8-103">Bạn sử dụng công cụ triển khai Office (ODT) để triển khai Office 365 Phiên bản Office.</span><span class="sxs-lookup"><span data-stu-id="545a8-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="545a8-104">Công cụ triển khai Office (Setup. exe) chạy từ dòng lệnh và sử dụng tệp XML cấu hình để xác định những cài đặt để áp dụng khi triển khai Office.</span><span class="sxs-lookup"><span data-stu-id="545a8-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="545a8-105">Tải xuống phiên bản mới nhất của công cụ triển khai Office từ [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="545a8-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="545a8-106">Sử dụng [công cụ Tuỳ chỉnh Office (Oct)](https://config.office.com) để chọn tuỳ chọn triển khai của bạn và tạo tệp XML cấu hình.</span><span class="sxs-lookup"><span data-stu-id="545a8-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="545a8-107">Xuất tập tin cấu hình và đặt nó cục bộ trên cùng một thư mục mà Setup. exe cư trú.</span><span class="sxs-lookup"><span data-stu-id="545a8-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="545a8-108">**Lưu ý:** Các vấn đề cài đặt Office thường xảy ra do các tệp cấu hình sai hoặc định dạng lại.</span><span class="sxs-lookup"><span data-stu-id="545a8-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="545a8-109">Để tránh các vấn đề như vậy, chúng tôi khuyên bạn sử dụng công cụ Tuỳ chỉnh Office để tạo tệp cấu hình.</span><span class="sxs-lookup"><span data-stu-id="545a8-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="545a8-110">Bạn cũng có thể nhập tệp cấu hình hiện có vào công cụ Tuỳ chỉnh Office.</span><span class="sxs-lookup"><span data-stu-id="545a8-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="545a8-111">Từ dấu nhắc lệnh nâng cao, chuyển sang vị trí mà Setup. exe cư trú và chạy công cụ triển khai Office trong chế độ tải xuống và chỉ định tệp cấu hình bạn vừa lưu.</span><span class="sxs-lookup"><span data-stu-id="545a8-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="545a8-112">Trong ví dụ này, tệp cấu hình được đặt tên configuration. xml:</span><span class="sxs-lookup"><span data-stu-id="545a8-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="545a8-113">Chạy công cụ triển khai Office trong chế độ cấu hình và chỉ định tệp cấu hình.</span><span class="sxs-lookup"><span data-stu-id="545a8-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="545a8-114">**Lưu ý:** Bạn phải chạy bước này từ máy khách mà bạn muốn cài đặt Office và bạn phải có quyền quản trị viên cục bộ trên máy tính.</span><span class="sxs-lookup"><span data-stu-id="545a8-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="545a8-115">Để tìm hiểu thêm về cách sử dụng công cụ triển khai Office cho Microsoft 365 ứng dụng cho các trường hợp triển khai doanh nghiệp, hãy xem [tổng quan về công cụ triển khai Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="545a8-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="545a8-116">Để biết thêm chi tiết về cách sử dụng công cụ Tuỳ chỉnh Office, hãy xem [tổng quan về công cụ Tuỳ chỉnh Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="545a8-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
