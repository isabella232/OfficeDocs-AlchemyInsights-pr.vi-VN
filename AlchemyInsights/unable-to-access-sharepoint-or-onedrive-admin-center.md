---
title: Không thể truy cập vào Trung tâm quản trị SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 627a4ef2900a6b9bbef7eb3f3a214ee7c371e354
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/12/2020
ms.locfileid: "44716477"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a><span data-ttu-id="a1d30-102">Không thể truy cập vào Trung tâm quản trị SharePoint hoặc OneDrive</span><span class="sxs-lookup"><span data-stu-id="a1d30-102">Unable to access SharePoint or OneDrive admin center</span></span>

- <span data-ttu-id="a1d30-103">Nếu trang web trung tâm quản trị SharePoint hoặc OneDrive của bạn không truy nhập được hoặc không khả dụng, có thể có sự cố dịch vụ tạm thời trong đó người dùng gặp phải các lỗi điều hướng hoặc chậm trễ liên tục khi truy cập các trang web SharePoint hoặc nội dung OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a1d30-103">If your SharePoint or OneDrive Admin center site is inaccessible or unavailable, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="a1d30-104">Kiểm tra [bảng điều khiển tình trạng dịch vụ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) để xem liệu tổ chức của bạn có bị ảnh hưởng hay không.</span><span class="sxs-lookup"><span data-stu-id="a1d30-104">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

- <span data-ttu-id="a1d30-105">Toàn cầu và SharePoint quản trị viên cần phải được gán một giấy phép SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a1d30-105">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="a1d30-106">Tài khoản mới được tạo chỉ được gán với giấy phép SharePoint hoặc vai trò quản trị có thể gặp phải sự cố truy cập SharePoint, như "truy cập bị từ chối" hoặc "người dùng không tìm thấy."</span><span class="sxs-lookup"><span data-stu-id="a1d30-106">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="a1d30-107">Xin vui lòng cho ít nhất 24 giờ để đồng bộ để hoàn thành trên toàn hệ thống của chúng tôi.</span><span class="sxs-lookup"><span data-stu-id="a1d30-107">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="a1d30-108">Chúng tôi hiểu rằng 24 giờ có thể có vẻ như một thời gian dài.</span><span class="sxs-lookup"><span data-stu-id="a1d30-108">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="a1d30-109">Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="a1d30-109">In many cases, we're already working on a solution.</span></span>

- <span data-ttu-id="a1d30-110">Người dùng đặc quyền Identity quản lý ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) có thể nhận được truy cập bị từ chối nếu cho phép truy cập thời gian cửa sổ là rất nhỏ, xem [truy cập từ chối tài khoản PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span><span class="sxs-lookup"><span data-stu-id="a1d30-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new))  users may receive access denied if allowed access time window is very small, see  [Access denied to PIM accounts](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span></span>