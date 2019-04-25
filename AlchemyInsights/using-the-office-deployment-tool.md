---
title: Bằng cách sử dụng công cụ triển khai văn phòng
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: c7e0e96f225030590fdd516eaf3115c93a6335b6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423205"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="f0b64-102">Bằng cách sử dụng công cụ triển khai văn phòng (ODT)</span><span class="sxs-lookup"><span data-stu-id="f0b64-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="f0b64-103">Bạn sử dụng công cụ triển khai văn phòng (ODT) để triển khai Office 365 các phiên bản của Office.</span><span class="sxs-lookup"><span data-stu-id="f0b64-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="f0b64-104">Công cụ triển khai văn phòng (setup.exe) chạy từ dòng lệnh và sử dụng một tập tin XML cấu hình để xác định những cài đặt để áp dụng khi triển khai các văn phòng.</span><span class="sxs-lookup"><span data-stu-id="f0b64-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="f0b64-105">Tải về phiên bản mới nhất của công cụ triển khai Office từ [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="f0b64-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="f0b64-106">Sử dụng [Công cụ Tuỳ chỉnh Office (OCT)](https://config.office.com) để chọn các tuỳ chọn triển khai của bạn và tạo ra các tệp tin XML cấu hình.</span><span class="sxs-lookup"><span data-stu-id="f0b64-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="f0b64-107">Xuất khẩu các tập tin cấu hình và đặt nó tại địa phương vào cùng một thư mục nơi cư trú của setup.exe.</span><span class="sxs-lookup"><span data-stu-id="f0b64-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="f0b64-108">**Lưu ý:** Văn phòng cài đặt vấn đề thường xảy ra do sai hoặc tập tin cấu hình malformatted.</span><span class="sxs-lookup"><span data-stu-id="f0b64-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="f0b64-109">Để tránh các vấn đề như vậy, chúng tôi khuyên bạn sử dụng công cụ Tuỳ chỉnh Office để tạo tập tin cấu hình.</span><span class="sxs-lookup"><span data-stu-id="f0b64-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="f0b64-110">Bạn cũng có thể nhập tập tin cấu hình sẵn có vào công cụ Tuỳ chỉnh Office.</span><span class="sxs-lookup"><span data-stu-id="f0b64-110">You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="f0b64-111">Từ một dấu nhắc lệnh nâng lên, chuyển sang vị trí nơi cư trú của setup.exe và chạy công cụ triển khai Office trong chế độ tải về và xác định tập tin cấu hình mà bạn chỉ cần lưu lại.</span><span class="sxs-lookup"><span data-stu-id="f0b64-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="f0b64-112">Trong ví dụ này, tập tin cấu hình được đặt tên Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="f0b64-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="f0b64-113">Chạy công cụ triển khai văn phòng trong cấu hình chế độ và chỉ định tập tin cấu hình.</span><span class="sxs-lookup"><span data-stu-id="f0b64-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="f0b64-114">**Lưu ý:** Bạn phải chạy bước này từ máy tính khách hàng mà bạn muốn cài đặt văn phòng và bạn phải có quyền quản trị cục bộ trên máy tính đó.</span><span class="sxs-lookup"><span data-stu-id="f0b64-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="f0b64-115">Để tìm hiểu thêm về cách sử dụng công cụ triển khai Office cho các tình huống triển khai Office 365 ProPlus của bạn, hãy xem [tổng quan về công cụ triển khai văn phòng](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="f0b64-115">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="f0b64-116">Để biết thêm chi tiết về cách sử dụng công cụ Tuỳ chỉnh Office, hãy xem [tổng quan về công cụ Tuỳ chỉnh Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="f0b64-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

