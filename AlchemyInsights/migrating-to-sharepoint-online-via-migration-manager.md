---
title: Di chuyển sang SharePoint trực tuyến qua trình quản lý di trú
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932378"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="f3536-102">Di chuyển sang SharePoint trực tuyến qua trình quản lý di trú</span><span class="sxs-lookup"><span data-stu-id="f3536-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="f3536-103">**Quan trọng**: nhiều SharePoint trực tuyến và OneDrive khách hàng chạy ứng dụng kinh doanh quan trọng đối với các dịch vụ chạy trong nền.</span><span class="sxs-lookup"><span data-stu-id="f3536-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f3536-104">Chúng bao gồm di chuyển nội dung, ngăn chặn mất dữ liệu (DLP) và giải pháp sao lưu.</span><span class="sxs-lookup"><span data-stu-id="f3536-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f3536-105">Trong những lần chưa từng có, chúng tôi đang thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn có hiệu quả cao và đáng tin cậy cho người dùng của bạn phụ thuộc vào dịch vụ hơn bao giờ hết trong các tình huống làm việc từ xa.</span><span class="sxs-lookup"><span data-stu-id="f3536-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f3536-106">Để hỗ trợ cho mục tiêu này, chúng tôi đã thực hiện các giới hạn điều chỉnh chặt chẽ hơn trên các ứng dụng nền (di chuyển, DLP và các giải pháp sao lưu) trong giờ ban ngày trong tuần.</span><span class="sxs-lookup"><span data-stu-id="f3536-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f3536-107">Bạn nên mong đợi rằng các ứng dụng này sẽ đạt được thông lượng rất hạn chế trong những thời gian này.</span><span class="sxs-lookup"><span data-stu-id="f3536-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f3536-108">Tuy nhiên, trong giờ tối và cuối tuần cho khu vực, Dịch vụ sẽ sẵn sàng xử lý số lượng yêu cầu cao hơn đáng kể từ ứng dụng nền.</span><span class="sxs-lookup"><span data-stu-id="f3536-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f3536-109">**Quản lý di chuyển**</span><span class="sxs-lookup"><span data-stu-id="f3536-109">**Migration Manager**</span></span>

<span data-ttu-id="f3536-110">Nằm trong Trung tâm quản trị SharePoint hiện đại, trình quản lý di chuyển hướng dẫn bạn thiết lập các khách hàng của bạn và tạo các tác vụ của bạn.</span><span class="sxs-lookup"><span data-stu-id="f3536-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="f3536-111">Bạn có thể chỉ định cài đặt chung hoặc cấp tác vụ, xem tiến trình công việc tất cả-lên và tải xuống tóm tắt tổng hợp và báo cáo cấp tác vụ.</span><span class="sxs-lookup"><span data-stu-id="f3536-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="f3536-112">Bắt đầu với trình quản lý di chuyển</span><span class="sxs-lookup"><span data-stu-id="f3536-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="f3536-113">Thiết lập trình quản lý di chuyển khách hàng</span><span class="sxs-lookup"><span data-stu-id="f3536-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- [<span data-ttu-id="f3536-114">Cài đặt trình quản lý di chuyển</span><span class="sxs-lookup"><span data-stu-id="f3536-114">Migration Manager Settings</span></span>](https://docs.microsoft.com/sharepointmigration/mm-settings)
