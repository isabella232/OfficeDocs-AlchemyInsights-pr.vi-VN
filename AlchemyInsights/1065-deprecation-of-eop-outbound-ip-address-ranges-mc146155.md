---
title: 1065 deprecation EOP outbound IP địa chỉ rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28320488"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="7e2ad-102">Deprecation EOP ra ngoài phạm vi địa chỉ IP</span><span class="sxs-lookup"><span data-stu-id="7e2ad-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="7e2ad-p101">Chúng tôi đã phát hiện một vấn đề tiềm năng với các tổ chức của bạn (nếu không được sửa chữa bởi 26 tháng 10 năm 2018) có thể phá vỡ luồng thư đến chỗ hoặc bên ngoài các điểm đến của bạn. Như là trước đó đã truyền đạt, để đơn giản hóa quản lý phạm vi địa chỉ IP, chúng tôi đang củng cố các dải địa chỉ IP bảo vệ trực tuyến trao đổi (EOP), được sử dụng để gửi và nhận thư điện tử bên ngoài của Office 365. Phân tích của chúng tôi cho thấy rằng một hoặc nhiều e-mail bên ngoài nguồn hoặc điểm đến mà bạn đã đặt cấu hình trong thư lưu lượng kết nối không chấp nhận kết nối từ IP địa chỉ phạm vi Hiển thị [ở đây](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="7e2ad-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="7e2ad-106">Hoạt động trước ngày 26 tháng 10 để đảm bảo các nguồn và các điểm đến sẽ chấp nhận kết nối đến và đi từ tất cả [xuất bản EOP IP địa chỉ](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="7e2ad-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="7e2ad-107">Để biết thêm chi tiết về sự thay đổi này, hãy xem Trung tâm thông báo bài viết [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)hoặc [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="7e2ad-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="7e2ad-p102">**Lưu ý**: nếu trước đây bạn sử dụng IP hoặc URL xuất bản thông qua HTML, XML, và RSS endpoint Cập Nhật, bạn cũng nên di chuyển sử dụng các dịch vụ web mới cho các loại bản cập nhật tự động. Để biết thêm chi tiết, hãy xem [Office 365 endpoint thể loại và Office 365 địa chỉ IP và URL trang web dịch vụ](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="7e2ad-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

