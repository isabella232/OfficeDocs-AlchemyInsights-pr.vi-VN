---
title: Triển khai phần bổ trợ cho mọi Ứng dụng Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/30/2021
ms.locfileid: "52125808"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="a210b-102">Triển khai phần bổ trợ cho mọi Ứng dụng Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a210b-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="a210b-103">Triển khai tập trung là cách được đề xuất để triển khai Office bổ trợ cho người dùng và nhóm trong tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="a210b-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="a210b-104">Để triển khai các phần bổ trợ, hãy làm theo các bước dưới đây:</span><span class="sxs-lookup"><span data-stu-id="a210b-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="a210b-105">**Lưu ý:** Để cài đặt các phần bổ trợ dành cho Office người dùng cá nhân, hãy xem mục Xem, quản lý và cài đặt phần bổ trợ [trong Office trình.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="a210b-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="a210b-106">Ngoài ra, hãy đảm bảo đã bật tính năng mua riêng Office Store của Store.</span><span class="sxs-lookup"><span data-stu-id="a210b-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> 

1. <span data-ttu-id="a210b-107">Đảm bảo rằng môi trường của bạn đáp ứng các yêu cầu về triển khai phần bổ trợ sử dụng Triển khai Tập trung.</span><span class="sxs-lookup"><span data-stu-id="a210b-107">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="a210b-108">Để biết chi tiết, hãy xem [Yêu cầu](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="a210b-108">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="a210b-109">Đi tới Cài đặt **Tích**  >  **hợp Tải** ứng  >  **dụng** trong trung tâm quản trị Microsoft 365 để triển khai các phần bổ trợ.</span><span class="sxs-lookup"><span data-stu-id="a210b-109">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="a210b-110">Lưu ý:</span><span class="sxs-lookup"><span data-stu-id="a210b-110">Notes:</span></span> 

- <span data-ttu-id="a210b-111">Ứng dụng Tích hợp yêu cầu người quản trị phải có quyền Quản trị Toàn cầu Exchange quản trị.</span><span class="sxs-lookup"><span data-stu-id="a210b-111">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="a210b-112">Khi triển khai các phần bổ trợ cho nhiều người dùng, chúng tôi khuyên bạn nên thực hiện gán bằng cách sử dụng các nhóm thay vì người dùng riêng lẻ.</span><span class="sxs-lookup"><span data-stu-id="a210b-112">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="a210b-113">Để biết chi tiết, [hãy xem mục Những điều cần cân nhắc khi gán phần bổ trợ cho người dùng và nhóm.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="a210b-113">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="a210b-114">Triển khai Tập trung không hỗ trợ người dùng trong các nhóm lồng hoặc các nhóm có nhóm cha mẹ.</span><span class="sxs-lookup"><span data-stu-id="a210b-114">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="a210b-115">Để biết chi tiết, [hãy xem mục Gán người dùng và nhóm.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="a210b-115">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="a210b-116">Đảm bảo rằng Dịch vụ Quản lý Ứng dụng Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') được kích hoạt để người dùng đăng nhập.</span><span class="sxs-lookup"><span data-stu-id="a210b-116">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="a210b-117">Để biết chi tiết, hãy xem [Cấu hình thuộc tính ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="a210b-117">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="a210b-118">Nếu bạn gặp sự cố khi triển khai phần bổ trợ bằng Cách sử dụng Ứng dụng Tích hợp, hãy thử triển khai bằng [Cách sử dụng Phần Bổ trợ.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="a210b-118">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="a210b-119">Để biết thêm thông tin, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="a210b-119">For more information, see:</span></span>

<span data-ttu-id="a210b-120">[Triển khai các phần bổ trợ trong trung tâm quản trị](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Quản lý phần bổ trợ trong trung tâm quản trị](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Sử dụng các lệnh ghép ngắn PowerShell Triển khai Tập trung để quản lý phần bổ trợ](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Phát hành Office bổ trợ bằng Triển khai Tập trung thông qua Trung tâm quản Microsoft 365 chính](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Khắc phục sự cố: Người dùng không nhìn thấy các phần bổ trợ](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Khắc phục lỗi người dùng Office Bổ trợ](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="a210b-120">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>