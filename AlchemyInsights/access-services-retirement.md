---
title: Truy cập Dịch vụ nghỉ hưu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687280"
---
# <a name="access-services-retirement"></a><span data-ttu-id="bdc2f-102">Truy cập Dịch vụ nghỉ hưu</span><span class="sxs-lookup"><span data-stu-id="bdc2f-102">Access services retirement</span></span>

<span data-ttu-id="bdc2f-103">Như chúng tôi ban đầu được công bố trong MC97576, vào tháng ba 2017, và tiếp tục giao tiếp trong năm qua truy cập Dịch vụ đang được nghỉ hưu.</span><span class="sxs-lookup"><span data-stu-id="bdc2f-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="bdc2f-104">Giai đoạn tiếp theo trong quá trình này sẽ là loại bỏ truy cập web cơ sở dữ liệu sử dụng danh sách SharePoint như lưu trữ dữ liệu cơ bản của họ.</span><span class="sxs-lookup"><span data-stu-id="bdc2f-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="bdc2f-105">**Điều này ảnh hưởng đến tôi như thế nào?**</span><span class="sxs-lookup"><span data-stu-id="bdc2f-105">**How does this affect me?**</span></span>

<span data-ttu-id="bdc2f-106">Bắt đầu từ ngày 2019 tháng 6, chúng tôi sẽ ngừng tạo cơ sở dữ liệu Access mới trong SharePoint Online và tắt dịch vụ và bất kỳ ứng dụng còn lại nào vào tháng 2020.</span><span class="sxs-lookup"><span data-stu-id="bdc2f-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="bdc2f-107">**Tôi cần làm gì để chuẩn bị cho sự thay đổi này?**</span><span class="sxs-lookup"><span data-stu-id="bdc2f-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="bdc2f-108">Chúng tôi khuyến khích bạn tạo một kế hoạch chuyển tiếp cho cơ sở dữ liệu Web Access của tổ chức bạn.</span><span class="sxs-lookup"><span data-stu-id="bdc2f-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="bdc2f-109">Quản trị viên có thể sử dụng [máy quét ứng dụng SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) để lấy hàng tồn kho của các ứng dụng truy cập mà các trang web đang sử dụng.</span><span class="sxs-lookup"><span data-stu-id="bdc2f-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="bdc2f-110">Có một số cách để di chuyển dữ liệu truy cập cơ sở dữ liệu web:</span><span class="sxs-lookup"><span data-stu-id="bdc2f-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="bdc2f-111">Nhập vào cơ sở dữ liệu Access cục bộ (. ACCDB) hoặc tệp Excel.</span><span class="sxs-lookup"><span data-stu-id="bdc2f-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="bdc2f-112">Chúng tôi cũng khuyên bạn nên khám phá Microsoft PowerApps như một nền tảng thay thế để tạo các giải pháp kinh doanh không có mã cho các thiết bị web và di động.</span><span class="sxs-lookup"><span data-stu-id="bdc2f-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>