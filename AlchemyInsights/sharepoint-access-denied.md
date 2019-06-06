---
title: Khắc phục sự cố truy cập từ chối các thư
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 5958ad06ca905f713b5f56aa5c536e95a485f01c
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735759"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="521b5-102">Khắc phục sự cố truy cập từ chối các thư</span><span class="sxs-lookup"><span data-stu-id="521b5-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="521b5-103">Nếu bạn nhận được quyền truy cập bị từ chối tin nhắn khi đang cố duyệt một trang web Sharepoint Online, xin vui lòng xem các bên dưới bài viết.</span><span class="sxs-lookup"><span data-stu-id="521b5-103">If you are receiving an access denied message when attempting to browse a Sharepoint Online site, please see the below articles.</span></span>

## <a name="add-and-license-the-user"></a><span data-ttu-id="521b5-104">Thêm và giấy phép người dùng</span><span class="sxs-lookup"><span data-stu-id="521b5-104">Add and License the user</span></span>

<span data-ttu-id="521b5-105">Đảm bảo rằng bạn [gán giấy phép cho người dùng trong Office 365 Beta dành cho doanh nghiệp](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="521b5-105">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>

<span data-ttu-id="521b5-106">Gán quyền</span><span class="sxs-lookup"><span data-stu-id="521b5-106">Assign Permissions</span></span>

<span data-ttu-id="521b5-107">Nếu người dùng đã được chỉ định một cấp phép Sharepoint và vẫn nhận được quyền truy cập bị từ chối thư, hãy đảm bảo rằng họ có [mức độ thích hợp cho phép gán](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="521b5-107">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level assigned](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>

<span data-ttu-id="521b5-108">Xem xét sử dụng các tính năng yêu cầu truy cập</span><span class="sxs-lookup"><span data-stu-id="521b5-108">Consider using the access request feature</span></span>

<span data-ttu-id="521b5-109">Các tính năng [yêu cầu quyền truy cập](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) cho phép mọi người để yêu cầu quyền truy cập vào nội dung mà họ hiện tại không có sự cho phép để xem.</span><span class="sxs-lookup"><span data-stu-id="521b5-109">The [access request](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) feature allows people to request access to content that they do not currently have permission to see.</span></span> 

<span data-ttu-id="521b5-110">Cho phép tùy chỉnh kịch bản có thể gây ra các quyền truy cập bị từ chối các vấn đề</span><span class="sxs-lookup"><span data-stu-id="521b5-110">Allow custom script may cause access denied issues</span></span>

<span data-ttu-id="521b5-111">Có những tình huống nhất định mà tính năng "Cho phép tùy chỉnh kịch bản" có thể trình bày một truy cập bị từ chối.</span><span class="sxs-lookup"><span data-stu-id="521b5-111">There are certain scenarios where the "Allow custom script" feature may be presenting an access denied.</span></span> <span data-ttu-id="521b5-112">Đối với một danh sách các tính năng ảnh hưởng, cân nhắc an ninh và khả năng vô hiệu hóa các tính năng.</span><span class="sxs-lookup"><span data-stu-id="521b5-112">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="521b5-113">Xin vui lòng truy cập vào, [cho phép hoặc ngăn chặn các tuỳ chỉnh script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="521b5-113">Please visit , [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)</span></span>

<span data-ttu-id="521b5-114">Lưu ý: Nếu một trang web OneDrive hoặc SharePoint không phải là có sẵn cho nhiều người dùng trước đó đã truy cập, có thể có một vấn đề tạm thời dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="521b5-114">Note: If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="521b5-115">[Kiểm tra bảng điều khiển dịch vụ y tế](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="521b5-115">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


  

