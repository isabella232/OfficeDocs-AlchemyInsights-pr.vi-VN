---
title: Bằng cách sử dụng công cụ triển khai văn phòng
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28320888"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="b7e26-102">Bằng cách sử dụng công cụ triển khai văn phòng (ODT)</span><span class="sxs-lookup"><span data-stu-id="b7e26-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="b7e26-p101">Bạn sử dụng công cụ triển khai văn phòng (ODT) để triển khai Office 365 các phiên bản của Office. Công cụ triển khai văn phòng (setup.exe) chạy từ dòng lệnh và sử dụng một tập tin XML cấu hình để xác định những cài đặt để áp dụng khi triển khai các văn phòng.</span><span class="sxs-lookup"><span data-stu-id="b7e26-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="b7e26-105">Tải về phiên bản mới nhất của công cụ triển khai Office từ [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="b7e26-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="b7e26-p102">Sử dụng [Công cụ Tuỳ chỉnh Office (OCT)](https://config.office.com) để chọn các tuỳ chọn triển khai của bạn và tạo ra các tệp tin XML cấu hình. Xuất khẩu các tập tin cấu hình và đặt nó tại địa phương vào cùng một thư mục nơi cư trú của setup.exe.</span><span class="sxs-lookup"><span data-stu-id="b7e26-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="b7e26-p103">**Lưu ý:** Văn phòng cài đặt vấn đề thường xảy ra do sai hoặc tập tin cấu hình malformatted. Để tránh các vấn đề như vậy, chúng tôi khuyên bạn sử dụng công cụ Tuỳ chỉnh Office để tạo tập tin cấu hình. Bạn cũng có thể nhập tập tin cấu hình sẵn có vào công cụ Tuỳ chỉnh Office.</span><span class="sxs-lookup"><span data-stu-id="b7e26-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="b7e26-p104">Từ một dấu nhắc lệnh nâng lên, chuyển sang vị trí nơi cư trú của setup.exe và chạy công cụ triển khai Office trong chế độ tải về và xác định tập tin cấu hình mà bạn chỉ cần lưu lại. Trong ví dụ này, tập tin cấu hình được đặt tên Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="b7e26-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="b7e26-113">Chạy công cụ triển khai văn phòng trong cấu hình chế độ và chỉ định tập tin cấu hình.</span><span class="sxs-lookup"><span data-stu-id="b7e26-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="b7e26-114">**Lưu ý:** Bạn phải chạy bước này từ máy tính khách hàng mà bạn muốn cài đặt văn phòng và bạn phải có quyền quản trị cục bộ trên máy tính đó.</span><span class="sxs-lookup"><span data-stu-id="b7e26-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="b7e26-p105">Để tìm hiểu thêm về cách sử dụng công cụ triển khai Office cho các tình huống triển khai Office 365 ProPlus của bạn, hãy xem [tổng quan về công cụ triển khai văn phòng](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Để biết thêm chi tiết về cách sử dụng công cụ Tuỳ chỉnh Office, hãy xem [tổng quan về công cụ Tuỳ chỉnh Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="b7e26-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

