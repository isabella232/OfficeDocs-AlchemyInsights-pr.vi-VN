---
title: 1065 sự phản kháng của địa chỉ IP đi EOP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704619"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="7b3a2-102">Sự phản kháng của dải địa chỉ IP đi EOP</span><span class="sxs-lookup"><span data-stu-id="7b3a2-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="7b3a2-103">Chúng tôi đã phát hiện một vấn đề tiềm ẩn với tổ chức của bạn (nếu không được sửa chữa bởi ngày 26 tháng 10, 2018) có thể phá vỡ luồng thư đến các điểm đến tại chỗ hoặc bên ngoài của bạn.</span><span class="sxs-lookup"><span data-stu-id="7b3a2-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="7b3a2-104">Như đã truyền đạt, để đơn giản hóa quản lý phạm vi địa chỉ IP, chúng tôi đang củng cố phạm vi địa chỉ IP Exchange Online Protection (EOP) được sử dụng để gửi và nhận email bên ngoài Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7b3a2-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="7b3a2-105">Phân tích của chúng tôi chỉ ra rằng một hoặc nhiều nguồn email bên ngoài hoặc các điểm đến mà bạn đã cấu hình trong kết nối luồng thư không chấp nhận kết nối từ phạm vi địa chỉ IP được hiển thị [ở đây](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="7b3a2-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="7b3a2-106">Hành động trước ngày 26 tháng 10 để đảm bảo các nguồn và các điểm đến sẽ chấp nhận các kết nối đến và đi từ tất cả các [địa chỉ IP EOP xuất bản](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="7b3a2-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="7b3a2-107">Để biết thêm thông tin về thay đổi này, vui lòng xem Trung tâm thông báo bài viết [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)hoặc [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="7b3a2-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="7b3a2-108">**Lưu ý**: nếu bạn đã sử dụng IP hoặc URL xuất bản qua HTML, XML và RSS để cập nhật điểm cuối, bạn cũng nên di chuyển sang các dịch vụ web mới để tự động hoá các loại bản Cập Nhật.</span><span class="sxs-lookup"><span data-stu-id="7b3a2-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="7b3a2-109">Để biết thêm thông tin, xem [microsoft 365 điểm cuối danh mục và microsoft 365 địa chỉ IP và URL web dịch vụ](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="7b3a2-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
