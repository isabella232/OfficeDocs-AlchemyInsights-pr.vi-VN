---
title: Throttling SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773869"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="34477-102">Throttling SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="34477-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="34477-103">**Quan trọng**: trong những thời gian chưa từng có này, chúng tôi sẽ thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn sẵn có – vui lòng truy cập vào các điều [chỉnh tính năng tạm thời trong SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="34477-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="34477-104">**máy chủ 503 là lỗi bận**</span><span class="sxs-lookup"><span data-stu-id="34477-104">**503 server is busy error**</span></span>

<span data-ttu-id="34477-105">Người dùng có thể nhận được một máy chủ 503 là lỗi bận rộn khi tìm cách dẫn hướng đến các site SharePoint hoặc OneDrive.</span><span class="sxs-lookup"><span data-stu-id="34477-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="34477-106">Lỗi này có thể được gây ra bởi điều chỉnh bên trong dịch vụ SharePoint.</span><span class="sxs-lookup"><span data-stu-id="34477-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="34477-107">SharePoint Online sử dụng điều chỉnh để duy trì hiệu năng và độ tin cậy tối ưu của dịch vụ SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="34477-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="34477-108">Throttling giới hạn số lượng hành động của người dùng hoặc cuộc gọi đồng thời (theo script hoặc mã) để ngăn chặn việc sử dụng tài nguyên.</span><span class="sxs-lookup"><span data-stu-id="34477-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="34477-109">Để biết thêm thông tin về việc xem thử điều chỉnh, [tránh bị Throttled hoặc bị chặn trong SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="34477-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="34477-110">Nếu bạn cho rằng lỗi này không liên quan đến throttling, bạn có thể kiểm tra xem liệu có hoạt động bảo trì nào xảy ra trên đối tượng thuê của bạn bằng cách dẫn hướng đến [Trung tâm thông báo](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="34477-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="34477-111">Cuối cùng, hãy đảm bảo bạn truy nhập trang trạng thái [dịch vụ](https://portal.office.com/adminportal/home#/servicehealth) để kiểm tra các sự cố/sự cố có thể xảy ra.</span><span class="sxs-lookup"><span data-stu-id="34477-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

