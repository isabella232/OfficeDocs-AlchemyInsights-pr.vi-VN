---
title: Truy cập vào dịch vụ hưu trí
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 5f171050479f34077f3dc155bec40437f86b84c0
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35359395"
---
# <a name="access-services-retirement"></a><span data-ttu-id="872cd-102">Truy cập vào dịch vụ hưu trí</span><span class="sxs-lookup"><span data-stu-id="872cd-102">Access services retirement</span></span>

<span data-ttu-id="872cd-103">Như chúng tôi ban đầu được công bố trong MC97576, vào tháng 3 năm 2017, và tiếp tục để giao tiếp trong những năm qua dịch vụ truy cập đang bị rút lui khỏi Office 365.</span><span class="sxs-lookup"><span data-stu-id="872cd-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="872cd-104">Giai đoạn tiếp theo trong quá trình này sẽ loại bỏ các quyền truy cập cơ sở dữ liệu Web mà sử dụng danh sách SharePoint như là của họ lưu trữ dữ liệu nằm bên dưới.</span><span class="sxs-lookup"><span data-stu-id="872cd-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="872cd-105">**Làm thế nào để điều này ảnh hưởng đến tôi?**</span><span class="sxs-lookup"><span data-stu-id="872cd-105">**How does this affect me?**</span></span>

<span data-ttu-id="872cd-106">Bắt đầu từ tháng sáu 2019, chúng tôi sẽ ngừng các sáng tạo mới truy cập cơ sở dữ liệu trong SharePoint Online và tắt các dịch vụ và bất kỳ ứng dụng còn lại của tháng tư năm 2020.</span><span class="sxs-lookup"><span data-stu-id="872cd-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="872cd-107">**Những gì tôi cần làm để chuẩn bị cho sự thay đổi này?**</span><span class="sxs-lookup"><span data-stu-id="872cd-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="872cd-108">Chúng tôi khuyến khích bạn tạo ra một kế hoạch chuyển đổi cho tổ chức của bạn truy cập trang web cơ sở dữ liệu.</span><span class="sxs-lookup"><span data-stu-id="872cd-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="872cd-109">Quản trị viên có thể sử dụng [SharePoint truy cập ứng dụng quét](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) để có một hàng tồn kho của các ứng dụng truy cập các trang web đang sử dụng.</span><span class="sxs-lookup"><span data-stu-id="872cd-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="872cd-110">Có rất nhiều cách để di chuyển các dữ liệu cơ sở dữ liệu truy cập web:</span><span class="sxs-lookup"><span data-stu-id="872cd-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="872cd-111">Nhập khẩu để cơ sở dữ liệu truy cập địa phương (. ACCDB) hoặc vào một tập tin Excel.</span><span class="sxs-lookup"><span data-stu-id="872cd-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="872cd-112">Chúng tôi cũng khuyên bạn nên khám phá Microsoft PowerApps như là một nền tảng thay thế để tạo ra không có mã số doanh nghiệp giải pháp cho web và các thiết bị di động.</span><span class="sxs-lookup"><span data-stu-id="872cd-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>