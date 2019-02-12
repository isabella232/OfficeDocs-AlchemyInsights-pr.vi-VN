---
title: 1554 Winsock lỗi 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903142"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="54735-102">Winsock lỗi 10061</span><span class="sxs-lookup"><span data-stu-id="54735-102">Winsock error 10061</span></span>

<span data-ttu-id="54735-p101">Mã lỗi này có nghĩa rằng Office 365 không thể thiết lập một cổng TCP (kết nối) với máy chủ mục tiêu. Nguyên nhân có thể nhất của lỗi này là một vấn đề với cấu hình tường lửa của bạn. Để khắc phục vấn đề, hãy kiểm tra các cài đặt này:</span><span class="sxs-lookup"><span data-stu-id="54735-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="54735-106">Xác minh cấu hình tường lửa của bạn với các thông tin trong [Office 365 URL và dải địa chỉ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="54735-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="54735-107">Nếu lỗi cụ thể để bảo vệ trực tuyến trao đổi (EOP), bạn nên đã được trước đó thông báo để thay đổi [địa chỉ IP bảo vệ trực tuyến trao đổi](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="54735-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="54735-108">Xác minh rằng nhà cung cấp dịch vụ Internet (ISP) không phải là chặn cổng.</span><span class="sxs-lookup"><span data-stu-id="54735-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="54735-109">Xác minh các thông minh chủ và mục tiêu máy chủ cài đặt kết nối của bạn.</span><span class="sxs-lookup"><span data-stu-id="54735-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="54735-110">Lưu ý rằng Office 365 không chặn *các* kết nối theo cách này.</span><span class="sxs-lookup"><span data-stu-id="54735-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

