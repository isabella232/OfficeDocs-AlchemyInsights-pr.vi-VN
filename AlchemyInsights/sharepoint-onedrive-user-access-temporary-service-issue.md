---
title: Vấn đề hiệu suất-SharePoint hoặc OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719538"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="057b4-102">SharePoint hoặc OneDrive chậm, không thể tiếp cận hoặc không sẵn dùng cho nhiều người dùng</span><span class="sxs-lookup"><span data-stu-id="057b4-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="057b4-103">Nếu một trang web OneDrive hoặc SharePoint không phải là có sẵn cho nhiều người dùng trước đó đã truy cập, có thể có một vấn đề tạm thời dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="057b4-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="057b4-104">[Kiểm tra bảng điều khiển dịch vụ y tế](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="057b4-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

## <a name="add-and-license-the-user"></a><span data-ttu-id="057b4-105">Thêm và giấy phép người dùng</span><span class="sxs-lookup"><span data-stu-id="057b4-105">Add and license the user</span></span>

<span data-ttu-id="057b4-106">Đảm bảo rằng bạn [gán giấy phép cho người dùng trong Office 365 Beta dành cho doanh nghiệp](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="057b4-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


## <a name="assign-permissions"></a><span data-ttu-id="057b4-107">Gán quyền</span><span class="sxs-lookup"><span data-stu-id="057b4-107">Assign Permissions</span></span>

<span data-ttu-id="057b4-108">Nếu người dùng đã được chỉ định một cấp phép Sharepoint và vẫn nhận được quyền truy cập bị từ chối thư, hãy đảm bảo rằng họ có [sự cho phép thích hợp cấp](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) được chỉ định.</span><span class="sxs-lookup"><span data-stu-id="057b4-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) assigned.</span></span>

## <a name="consider-using-the-access-request-feature"></a><span data-ttu-id="057b4-109">Xem xét sử dụng các tính năng yêu cầu truy cập</span><span class="sxs-lookup"><span data-stu-id="057b4-109">Consider using the access request feature</span></span>

<span data-ttu-id="057b4-110">[Truy cập yêu cầu tính năng](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) cho phép người để yêu cầu quyền truy cập vào nội dung mà họ hiện tại không có sự cho phép để xem.</span><span class="sxs-lookup"><span data-stu-id="057b4-110">The [access request feature](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

## <a name="allow-custom-script-may-cause-access-denied-issues"></a><span data-ttu-id="057b4-111">Cho phép tùy chỉnh kịch bản có thể gây ra các quyền truy cập bị từ chối các vấn đề</span><span class="sxs-lookup"><span data-stu-id="057b4-111">Allow custom script may cause access denied issues</span></span>

<span data-ttu-id="057b4-112">Có những tình huống nhất định mà các tính năng *cho phép tùy chỉnh kịch bản* có thể trình bày một truy cập bị từ chối.</span><span class="sxs-lookup"><span data-stu-id="057b4-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="057b4-113">Đối với một danh sách các tính năng ảnh hưởng, cân nhắc an ninh và khả năng vô hiệu hóa các tính năng.</span><span class="sxs-lookup"><span data-stu-id="057b4-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="057b4-114">Xin vui lòng ghé thăm [cho phép hoặc ngăn chặn các tuỳ chỉnh script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="057b4-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>
