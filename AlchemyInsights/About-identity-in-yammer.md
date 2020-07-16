---
title: Về danh tính trong yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148422"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="eef7d-102">Về danh tính trong yammer</span><span class="sxs-lookup"><span data-stu-id="eef7d-102">About identity in Yammer</span></span>

<span data-ttu-id="eef7d-103">Đó là khuyến cáo rằng tất cả các mạng thực hiện các bước sau để tránh các vấn đề liên quan đến danh tính:</span><span class="sxs-lookup"><span data-stu-id="eef7d-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="eef7d-104">Thực thi Office 365 nhận dạng sau khi cung cấp tài khoản Microsoft 365 cho người dùng Azure AD để đảm bảo rằng tất cả người dùng đăng nhập bằng cách sử dụng tài khoản Microsoft 365 chính.</span><span class="sxs-lookup"><span data-stu-id="eef7d-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="eef7d-105">Để biết thêm thông tin, xem [thi hành Office 365 nhận dạng cho người dùng yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="eef7d-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="eef7d-106">Củng cố nhiều yammer mạng.</span><span class="sxs-lookup"><span data-stu-id="eef7d-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="eef7d-107">Cấu hình kế thừa yammer cho phép nhiều mạng yammer được kết nối với một đối tượng thuê.</span><span class="sxs-lookup"><span data-stu-id="eef7d-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="eef7d-108">Để biết thêm thông tin, xem [di chuyển mạng-hợp nhất nhiều yammer mạng](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="eef7d-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="eef7d-109">Tùy chọn, thực thi cấp phép cho yammer để chặn người dùng từ yammer nếu họ không có giấy phép.</span><span class="sxs-lookup"><span data-stu-id="eef7d-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="eef7d-110">Để biết thêm thông tin, xem [quản lý giấy phép người dùng yammer trong Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="eef7d-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="eef7d-111">Cuối cùng, kiểm tra danh sách người dùng cho mạng yammer cũ và tạm ngưng người dùng hợp lệ.</span><span class="sxs-lookup"><span data-stu-id="eef7d-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="eef7d-112">Chúng tôi đề nghị bạn tạm ngưng (Hủy kích hoạt) người dùng thay vì xóa chúng, vì xóa là không thể đảo ngược.</span><span class="sxs-lookup"><span data-stu-id="eef7d-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="eef7d-113">Để biết thêm thông tin, xem [kiểm tra yammer người dùng trong mạng kết nối với Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) và [loại bỏ người dùng](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="eef7d-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="eef7d-114">Bằng cách đặt cấu hình yammer bằng các bước này, bạn cũng sẽ sẵn sàng cấu hình mạng yammer cho chế độ riêng dành cho Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="eef7d-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="eef7d-115">Để biết thêm thông tin, hãy xem [cấu hình mạng yammer của bạn cho chế độ riêng cho Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="eef7d-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>