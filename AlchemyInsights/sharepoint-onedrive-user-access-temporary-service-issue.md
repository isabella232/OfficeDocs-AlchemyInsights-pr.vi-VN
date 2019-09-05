---
title: Vấn đề hiệu suất-SharePoint hoặc OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 7e218cfff81274cd16d55dec2c5243eb8b74a3b7
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750578"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="5f0c2-102">SharePoint hoặc OneDrive chậm, không thể truy nhập hoặc không khả dụng cho nhiều người dùng</span><span class="sxs-lookup"><span data-stu-id="5f0c2-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="5f0c2-103">Nếu một trang web OneDrive hoặc SharePoint không có sẵn cho nhiều người dùng đã có quyền truy cập, có thể có một vấn đề dịch vụ tạm thời.</span><span class="sxs-lookup"><span data-stu-id="5f0c2-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="5f0c2-104">[Kiểm tra bảng điều khiển tình trạng dịch vụ](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="5f0c2-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="5f0c2-105">**Thêm và giấy phép người dùng**</span><span class="sxs-lookup"><span data-stu-id="5f0c2-105">**Add and license the user**</span></span>

<span data-ttu-id="5f0c2-106">Đảm bảo rằng bạn [gán giấy phép cho người dùng trong Office 365 cho doanh nghiệp](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="5f0c2-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="5f0c2-107">**Gán quyền**</span><span class="sxs-lookup"><span data-stu-id="5f0c2-107">**Assign Permissions**</span></span>

<span data-ttu-id="5f0c2-108">Nếu người dùng đã được gán một giấy phép SharePoint và vẫn nhận được thông báo từ chối truy cập, hãy đảm bảo rằng họ có [cấp quyền thích hợp](https://docs.microsoft.com/sharepoint/understanding-permission-levels) chỉ định.</span><span class="sxs-lookup"><span data-stu-id="5f0c2-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="5f0c2-109">**Xem xét sử dụng tính năng yêu cầu truy cập**</span><span class="sxs-lookup"><span data-stu-id="5f0c2-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="5f0c2-110">[Tính năng yêu cầu truy cập](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) cho phép người khác yêu cầu quyền truy cập vào nội dung mà họ hiện không có quyền xem.</span><span class="sxs-lookup"><span data-stu-id="5f0c2-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="5f0c2-111">**Cho phép tập lệnh tùy chỉnh có thể gây ra sự cố truy nhập bị từ chối**</span><span class="sxs-lookup"><span data-stu-id="5f0c2-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="5f0c2-112">Có một số trường hợp nơi *cho phép tính năng kịch bản tuỳ chỉnh* có thể trình bày truy cập bị từ chối.</span><span class="sxs-lookup"><span data-stu-id="5f0c2-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="5f0c2-113">Để có danh sách các tính năng bị ảnh hưởng, cân nhắc bảo mật và khả năng vô hiệu hóa tính năng.</span><span class="sxs-lookup"><span data-stu-id="5f0c2-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="5f0c2-114">Vui lòng truy cập [cho phép hoặc ngăn chặn tập lệnh tùy chỉnh](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="5f0c2-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

