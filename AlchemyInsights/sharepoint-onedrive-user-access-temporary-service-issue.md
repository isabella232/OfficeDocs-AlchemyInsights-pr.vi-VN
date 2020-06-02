---
title: Vấn đề hiệu suất-SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2dc0cd5f1641298853443d364eb9434ec1d9cd5a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511170"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="a1aa5-102">SharePoint hoặc OneDrive chậm, không thể truy nhập hoặc không khả dụng cho nhiều người dùng</span><span class="sxs-lookup"><span data-stu-id="a1aa5-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="a1aa5-103">Nếu một trang web OneDrive hoặc SharePoint không có sẵn cho nhiều người dùng đã có quyền truy cập, có thể có một vấn đề dịch vụ tạm thời.</span><span class="sxs-lookup"><span data-stu-id="a1aa5-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="a1aa5-104">[Kiểm tra bảng điều khiển tình trạng dịch vụ](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="a1aa5-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="a1aa5-105">**Thêm và giấy phép người dùng**</span><span class="sxs-lookup"><span data-stu-id="a1aa5-105">**Add and license the user**</span></span>

<span data-ttu-id="a1aa5-106">Đảm bảo rằng bạn [gán giấy phép cho người dùng trong Microsoft 365 cho doanh nghiệp](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="a1aa5-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="a1aa5-107">**Gán quyền**</span><span class="sxs-lookup"><span data-stu-id="a1aa5-107">**Assign Permissions**</span></span>

<span data-ttu-id="a1aa5-108">Nếu người dùng đã được gán một giấy phép SharePoint và vẫn nhận được thông báo từ chối truy cập, hãy đảm bảo rằng họ có [cấp quyền thích hợp](https://docs.microsoft.com/sharepoint/understanding-permission-levels) chỉ định.</span><span class="sxs-lookup"><span data-stu-id="a1aa5-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="a1aa5-109">**Xem xét sử dụng tính năng yêu cầu truy cập**</span><span class="sxs-lookup"><span data-stu-id="a1aa5-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="a1aa5-110">[Tính năng yêu cầu truy cập](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) cho phép người khác yêu cầu quyền truy cập vào nội dung mà họ hiện không có quyền xem.</span><span class="sxs-lookup"><span data-stu-id="a1aa5-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="a1aa5-111">**Cho phép tập lệnh tùy chỉnh có thể gây ra sự cố truy nhập bị từ chối**</span><span class="sxs-lookup"><span data-stu-id="a1aa5-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="a1aa5-112">Có một số trường hợp nơi *cho phép tính năng kịch bản tuỳ chỉnh* có thể trình bày truy cập bị từ chối.</span><span class="sxs-lookup"><span data-stu-id="a1aa5-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="a1aa5-113">Để có danh sách các tính năng bị ảnh hưởng, cân nhắc bảo mật và khả năng vô hiệu hóa tính năng.</span><span class="sxs-lookup"><span data-stu-id="a1aa5-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="a1aa5-114">Vui lòng truy cập [cho phép hoặc ngăn chặn tập lệnh tùy chỉnh](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="a1aa5-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

