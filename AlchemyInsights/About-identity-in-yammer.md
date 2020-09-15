---
title: Giới thiệu về danh tính trong yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664192"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="7e5b0-102">Giới thiệu về danh tính trong yammer</span><span class="sxs-lookup"><span data-stu-id="7e5b0-102">About identity in Yammer</span></span>

<span data-ttu-id="7e5b0-103">Khuyên rằng tất cả các mạng sẽ thực hiện các bước sau đây để tránh các vấn đề liên quan đến căn cước:</span><span class="sxs-lookup"><span data-stu-id="7e5b0-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="7e5b0-104">Áp dụng định danh Office 365 sau khi cung cấp tài khoản Microsoft 365 cho người dùng trong Azure AD để đảm bảo rằng tất cả người dùng đăng nhập bằng tài khoản Microsoft 365 chính của họ.</span><span class="sxs-lookup"><span data-stu-id="7e5b0-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="7e5b0-105">Để biết thêm thông tin, hãy xem thực [thi định danh Office 365 cho người dùng yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="7e5b0-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="7e5b0-106">Hợp nhất nhiều mạng yammer.</span><span class="sxs-lookup"><span data-stu-id="7e5b0-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="7e5b0-107">Cấu hình yammer kế thừa cho phép nhiều mạng yammer được kết nối với một đối tượng thuê.</span><span class="sxs-lookup"><span data-stu-id="7e5b0-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="7e5b0-108">Để biết thêm thông tin, hãy xem mục [di chuyển mạng-hợp nhất nhiều mạng yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="7e5b0-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="7e5b0-109">Bạn có thể thực thi cấp phép cho yammer để chặn người dùng từ yammer nếu họ không có giấy phép.</span><span class="sxs-lookup"><span data-stu-id="7e5b0-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="7e5b0-110">Để biết thêm thông tin, hãy xem [quản lý giấy phép người dùng yammer trong Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="7e5b0-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="7e5b0-111">Cuối cùng, hãy kiểm tra danh sách người dùng cho mạng yammer cũ hơn và tạm ngừng người dùng thừa kế.</span><span class="sxs-lookup"><span data-stu-id="7e5b0-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="7e5b0-112">Bạn nên tạm ngừng (Hủy kích hoạt) người dùng thay vì xóa chúng, vì việc xóa bỏ không thể thay đổi.</span><span class="sxs-lookup"><span data-stu-id="7e5b0-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="7e5b0-113">Để biết thêm thông tin, hãy xem [kiểm tra người dùng yammer trong các mạng được kết nối với Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) và [loại bỏ người dùng](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="7e5b0-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="7e5b0-114">Bằng cách đặt cấu hình yammer bằng các bước này, bạn cũng sẽ sẵn sàng cấu hình mạng yammer của bạn cho chế độ bản địa cho Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7e5b0-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="7e5b0-115">Để biết thêm thông tin, hãy xem [đặt cấu hình mạng yammer của bạn cho chế độ bản địa cho Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="7e5b0-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>