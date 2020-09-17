---
title: 1065 lưu lại địa chỉ IP của EOP Outbound rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806817"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="9e6e8-102">Deprecation của dải địa chỉ IP đi đến EOP</span><span class="sxs-lookup"><span data-stu-id="9e6e8-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="9e6e8-103">Chúng tôi đã phát hiện ra một vấn đề tiềm ẩn với tổ chức của bạn (nếu không được sửa vào ngày 26 tháng 10, 2018) có thể ngắt dòng thư đến đích tại chỗ hoặc bên ngoài của bạn.</span><span class="sxs-lookup"><span data-stu-id="9e6e8-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="9e6e8-104">Như truyền đạt được trước đó, để đơn giản hóa việc quản lý dải địa chỉ IP, chúng tôi đang củng cố phạm vi địa chỉ IP của Exchange Online Protection (EOP) được dùng để gửi và nhận email bên ngoài Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9e6e8-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="9e6e8-105">Phân tích của chúng tôi cho biết một hoặc nhiều nguồn email bên ngoài hoặc các đích mà bạn đã cấu hình trong các đường kết nối dòng thư không chấp nhận kết nối từ dải địa chỉ IP được hiển thị [ở đây](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="9e6e8-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="9e6e8-106">Act trước ngày 26 tháng 10 để đảm bảo các nguồn và đích này sẽ chấp nhận kết nối đến và từ tất cả các [địa chỉ IP đã phát hành của EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="9e6e8-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="9e6e8-107">Để biết thêm thông tin về thay đổi này, vui lòng xem Trung tâm thông báo bài viết [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)hoặc [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="9e6e8-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="9e6e8-108">**Lưu ý**: nếu trước đó bạn đã sử dụng IP hoặc URL phát hành qua HTML, XML và RSS cho các bản Cập Nhật điểm cuối, bạn cũng nên di chuyển đến các dịch vụ web mới để tự động hóa các kiểu bản cập nhật này.</span><span class="sxs-lookup"><span data-stu-id="9e6e8-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="9e6e8-109">Để biết thêm thông tin, hãy xem [thể loại điểm cuối microsoft 365 và địa chỉ IP của microsoft 365 và dịch vụ web URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="9e6e8-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
