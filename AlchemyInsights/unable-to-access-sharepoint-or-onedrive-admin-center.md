---
title: Không thể truy nhập vào Trung tâm quản trị SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: a70b0708b325c5feaefec3d97c957086d7f62cc6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749500"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a><span data-ttu-id="c1af1-102">Không thể truy nhập vào Trung tâm quản trị SharePoint hoặc OneDrive</span><span class="sxs-lookup"><span data-stu-id="c1af1-102">Unable to access SharePoint or OneDrive admin center</span></span>

- <span data-ttu-id="c1af1-103">Nếu site SharePoint hoặc trung tâm quản trị OneDrive của bạn không thể truy nhập được hoặc không sẵn dùng, thì có thể có sự cố dịch vụ tạm thời mà người dùng gặp phải sự chậm trễ hoặc dẫn hướng lỗi khi truy nhập site SharePoint hoặc nội dung OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c1af1-103">If your SharePoint or OneDrive Admin center site is inaccessible or unavailable, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="c1af1-104">Kiểm tra [bảng điều khiển trạng thái dịch vụ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) để xem liệu tổ chức của bạn có bị ảnh hưởng không.</span><span class="sxs-lookup"><span data-stu-id="c1af1-104">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

- <span data-ttu-id="c1af1-105">Người quản trị toàn cầu và SharePoint cần được gán giấy phép SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c1af1-105">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="c1af1-106">Các tài khoản mới được tạo chỉ được gán với một giấy phép SharePoint hoặc vai trò quản trị có thể gặp sự cố khi truy nhập SharePoint, chẳng hạn như "Access bị từ chối" hoặc "không tìm thấy người dùng".</span><span class="sxs-lookup"><span data-stu-id="c1af1-106">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="c1af1-107">Xin vui lòng cung cấp ít nhất 24 giờ để đồng bộ để hoàn tất qua các hệ thống của chúng tôi.</span><span class="sxs-lookup"><span data-stu-id="c1af1-107">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="c1af1-108">Chúng tôi hiểu rằng 24 giờ có thể có vẻ như một thời gian dài.</span><span class="sxs-lookup"><span data-stu-id="c1af1-108">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="c1af1-109">Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="c1af1-109">In many cases, we're already working on a solution.</span></span>

- <span data-ttu-id="c1af1-110">Người dùng quản lý danh tính đặc quyền ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) có thể nhận được truy nhập bị từ chối nếu có phép cửa sổ thời gian truy nhập là rất nhỏ, hãy xem  [Access bị từ chối đến tài khoản PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span><span class="sxs-lookup"><span data-stu-id="c1af1-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new))  users may receive access denied if allowed access time window is very small, see  [Access denied to PIM accounts](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span></span>