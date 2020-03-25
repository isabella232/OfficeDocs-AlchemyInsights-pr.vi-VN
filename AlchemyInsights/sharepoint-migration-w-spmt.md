---
title: Di chuyển SharePoint với SPMT
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2594"
ms.openlocfilehash: e7719d1fc6dda0d5bd340775219401dade2933fe
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931572"
---
# <a name="sharepoint-migration-with-spmt"></a><span data-ttu-id="aeeca-102">Di chuyển SharePoint với SPMT</span><span class="sxs-lookup"><span data-stu-id="aeeca-102">SharePoint Migration with SPMT</span></span>

<span data-ttu-id="aeeca-103">**Quan trọng**: nhiều SharePoint trực tuyến và OneDrive khách hàng chạy ứng dụng kinh doanh quan trọng đối với các dịch vụ chạy trong nền.</span><span class="sxs-lookup"><span data-stu-id="aeeca-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="aeeca-104">Chúng bao gồm di chuyển nội dung, ngăn chặn mất dữ liệu (DLP) và giải pháp sao lưu.</span><span class="sxs-lookup"><span data-stu-id="aeeca-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="aeeca-105">Trong những lần chưa từng có, chúng tôi đang thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn có hiệu quả cao và đáng tin cậy cho người dùng của bạn phụ thuộc vào dịch vụ hơn bao giờ hết trong các tình huống làm việc từ xa.</span><span class="sxs-lookup"><span data-stu-id="aeeca-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="aeeca-106">Để hỗ trợ cho mục tiêu này, chúng tôi đã thực hiện các giới hạn điều chỉnh chặt chẽ hơn trên các ứng dụng nền (di chuyển, DLP và các giải pháp sao lưu) trong giờ ban ngày trong tuần.</span><span class="sxs-lookup"><span data-stu-id="aeeca-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="aeeca-107">Bạn nên mong đợi rằng các ứng dụng này sẽ đạt được thông lượng rất hạn chế trong những thời gian này.</span><span class="sxs-lookup"><span data-stu-id="aeeca-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="aeeca-108">Tuy nhiên, trong giờ tối và cuối tuần cho khu vực, Dịch vụ sẽ sẵn sàng xử lý số lượng yêu cầu cao hơn đáng kể từ ứng dụng nền.</span><span class="sxs-lookup"><span data-stu-id="aeeca-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="aeeca-109">**Công cụ di chuyển SharePoint**</span><span class="sxs-lookup"><span data-stu-id="aeeca-109">**SharePoint Migration Tool**</span></span>

<span data-ttu-id="aeeca-110">Được thiết kế để sử dụng cho các cuộc di chuyển khác nhau, từ bộ tệp nhỏ nhất đến quy mô lớn của doanh nghiệp di cư, công cụ di chuyển SharePoint sẽ cho phép bạn chuyển thông tin của bạn lên đám mây và tận dụng sự hợp tác mới nhất, trí thông minh và giải pháp bảo mật với Office 365.</span><span class="sxs-lookup"><span data-stu-id="aeeca-110">Designed to be used for migrations ranging from the smallest set of files to a large scale enterprise migration, the SharePoint Migration Tool will allow you to transfer your information to the cloud and take advantage of the newest collaboration, intelligence, and security solutions with Office 365.</span></span>

- [<span data-ttu-id="aeeca-111">Tải xuống và cài đặt công cụ di chuyển SharePoint</span><span class="sxs-lookup"><span data-stu-id="aeeca-111">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
- [<span data-ttu-id="aeeca-112">Khắc phục sự cố và lỗi SPMT phổ biến</span><span class="sxs-lookup"><span data-stu-id="aeeca-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
- [<span data-ttu-id="aeeca-113">Khắc phục sự cố cài đặt SPMT</span><span class="sxs-lookup"><span data-stu-id="aeeca-113">Troubleshooting SPMT installation issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues#troubleshooting-spmt-installation-issues)
