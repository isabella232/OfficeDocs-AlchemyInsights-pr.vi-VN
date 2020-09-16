---
title: Các vấn đề về hiệu suất-SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771923"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="4a50b-102">SharePoint hoặc OneDrive chậm, không thể truy nhập hoặc không có sẵn cho nhiều người dùng</span><span class="sxs-lookup"><span data-stu-id="4a50b-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="4a50b-103">SharePoint hoặc OneDrive có thể chậm, không thể truy nhập hoặc không sẵn dùng hoặc có thể hiển thị các lỗi không sẵn dùng hoặc 503, vì một vài lý do:</span><span class="sxs-lookup"><span data-stu-id="4a50b-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="4a50b-104">Nếu site SharePoint hoặc OneDrive của bạn chậm hoặc bị trì hoãn đối với nhiều người dùng, có thể có sự cố dịch vụ tạm thời mà người dùng gặp phải sự chậm trễ hoặc dẫn hướng lỗi khi truy nhập site SharePoint hoặc nội dung OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4a50b-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="4a50b-105">Kiểm tra [bảng điều khiển trạng thái dịch vụ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) để xem liệu tổ chức của bạn có bị ảnh hưởng không.</span><span class="sxs-lookup"><span data-stu-id="4a50b-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="4a50b-106">Người dùng có thể nhận được một *máy chủ 503 là lỗi bận rộn* khi tìm cách dẫn hướng đến các site SharePoint hoặc OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4a50b-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="4a50b-107">Lỗi này có thể được gây ra bởi điều chỉnh bên trong dịch vụ SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4a50b-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="4a50b-108">SharePoint Online sử dụng điều chỉnh để duy trì hiệu năng và độ tin cậy tối ưu của dịch vụ SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="4a50b-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="4a50b-109">Throttling giới hạn số lượng hành động của người dùng hoặc cuộc gọi đồng thời (theo script hoặc mã) để ngăn chặn việc sử dụng tài nguyên.</span><span class="sxs-lookup"><span data-stu-id="4a50b-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="4a50b-110">Để biết thêm thông tin về việc xem thử điều chỉnh, [tránh bị Throttled hoặc bị chặn trong SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="4a50b-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="4a50b-111">Nếu bạn **gặp sự hiệu** suất chậm với trang hoặc site SharePoint **hiện đại hoặc hiện đại** , hãy sử dụng [công cụ chẩn đoán trang](https://aka.ms/perftool) để phân tích các trang.</span><span class="sxs-lookup"><span data-stu-id="4a50b-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="4a50b-112">Nếu bạn vẫn còn trải nghiệm hiệu năng chậm chung, vui lòng xem lại các tài nguyên ở cuối bài viết này: [giới thiệu về hiệu năng Tuning cho SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="4a50b-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  