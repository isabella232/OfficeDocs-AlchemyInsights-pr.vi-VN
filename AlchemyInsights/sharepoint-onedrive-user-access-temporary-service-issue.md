---
title: Các vấn đề về hiệu suất-SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771266"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="8b981-102">SharePoint hoặc OneDrive chậm, không thể truy nhập hoặc không có sẵn cho nhiều người dùng</span><span class="sxs-lookup"><span data-stu-id="8b981-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="8b981-103">Nếu một site OneDrive hoặc SharePoint không sẵn dùng cho nhiều người dùng trước đây có quyền truy nhập, có thể có sự cố dịch vụ tạm thời.</span><span class="sxs-lookup"><span data-stu-id="8b981-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="8b981-104">[Kiểm tra bảng điều khiển trạng thái dịch vụ](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="8b981-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="8b981-105">**Thêm và cấp giấy phép cho người dùng**</span><span class="sxs-lookup"><span data-stu-id="8b981-105">**Add and license the user**</span></span>

<span data-ttu-id="8b981-106">Đảm bảo rằng bạn [gán giấy phép cho người dùng trong Microsoft 365 dành cho doanh nghiệp](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="8b981-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="8b981-107">**Gán quyền**</span><span class="sxs-lookup"><span data-stu-id="8b981-107">**Assign Permissions**</span></span>

<span data-ttu-id="8b981-108">Nếu người dùng đã được gán giấy phép SharePoint và vẫn nhận được một thông báo bị từ chối truy nhập, vui lòng đảm bảo họ có [cấp độ quyền thích hợp](https://docs.microsoft.com/sharepoint/understanding-permission-levels) được gán.</span><span class="sxs-lookup"><span data-stu-id="8b981-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="8b981-109">**Cân nhắc việc sử dụng tính năng yêu cầu truy nhập**</span><span class="sxs-lookup"><span data-stu-id="8b981-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="8b981-110">[Tính năng truy nhập yêu cầu](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) cho phép mọi người yêu cầu quyền truy nhập vào nội dung mà họ hiện không có quyền để xem.</span><span class="sxs-lookup"><span data-stu-id="8b981-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="8b981-111">**Cho phép script tùy chỉnh có thể khiến các vấn đề bị từ chối truy nhập**</span><span class="sxs-lookup"><span data-stu-id="8b981-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="8b981-112">Có những tình huống nhất định mà tính năng *cho phép script tùy chỉnh* có thể trình bày một truy nhập bị từ chối.</span><span class="sxs-lookup"><span data-stu-id="8b981-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="8b981-113">Để biết danh sách các tính năng bị ảnh hưởng, cân nhắc về bảo mật và khả năng vô hiệu hóa tính năng.</span><span class="sxs-lookup"><span data-stu-id="8b981-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="8b981-114">Vui lòng truy nhập [cho phép hoặc ngăn chặn kịch bản tùy chỉnh](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="8b981-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

