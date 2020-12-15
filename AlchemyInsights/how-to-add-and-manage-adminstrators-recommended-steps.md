---
title: Cách thêm và quản lý các bước được đề xuất
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678866"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a><span data-ttu-id="56c95-102">Cách thêm và quản lý các bước được đề xuất</span><span class="sxs-lookup"><span data-stu-id="56c95-102">How to add and manage adminstrators - recommended steps</span></span>

<span data-ttu-id="56c95-103">**Chỉnh sửa người quản trị đăng ký hoặc người quản trị**</span><span class="sxs-lookup"><span data-stu-id="56c95-103">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="56c95-104">Người quản trị tài khoản có thể chỉnh sửa cả hai vai trò trong khi người quản trị đăng ký chỉ có thể thay đổi đồng quản trị trong [cổng thông tin Azure](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="56c95-104">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="56c95-105">Thêm hoặc thay đổi người quản trị thuê bao Azure</span><span class="sxs-lookup"><span data-stu-id="56c95-105">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="56c95-106">**Cập Nhật người quản trị đăng ký hoặc Co-Administrator cho đăng ký nội bộ (phát sóng)**</span><span class="sxs-lookup"><span data-stu-id="56c95-106">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="56c95-107">Người quản trị dịch vụ hoặc đồng người quản trị có thể tự phục vụ hành động này bằng cách sử dụng các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="56c95-107">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="56c95-108">Đăng nhập vào [cổng thông tin Azure](https://ms.portal.azure.com/#home) và bấm **quản lý chi phí + thanh toán** trong lưỡi mũi trái.</span><span class="sxs-lookup"><span data-stu-id="56c95-108">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="56c95-109">Bấm vào mục dòng với đăng ký của bạn.</span><span class="sxs-lookup"><span data-stu-id="56c95-109">Click on the line item with your subscription.</span></span> <span data-ttu-id="56c95-110">Điều này sẽ mở tổng quan về đăng ký của bạn.</span><span class="sxs-lookup"><span data-stu-id="56c95-110">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="56c95-111">Trên lưỡi **đăng ký** , bấm **thuộc tính**.</span><span class="sxs-lookup"><span data-stu-id="56c95-111">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="56c95-112">Bấm vào nút **quản trị dịch vụ** .</span><span class="sxs-lookup"><span data-stu-id="56c95-112">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="56c95-113">Nhập email của người dùng mà bạn muốn đặt làm người quản trị dịch vụ và bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="56c95-113">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="56c95-114">**Thêm/thay đổi/loại bỏ đồng người quản trị**</span><span class="sxs-lookup"><span data-stu-id="56c95-114">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="56c95-115">Đăng nhập vào [cổng thông tin Azure](https://ms.portal.azure.com/#home) với tư cách là người quản trị dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="56c95-115">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="56c95-116">Mở [đăng ký](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) và chọn một thuê bao.</span><span class="sxs-lookup"><span data-stu-id="56c95-116">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="56c95-117">(Đồng quản trị chỉ có thể gán tại phạm vi thuê bao.)</span><span class="sxs-lookup"><span data-stu-id="56c95-117">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="56c95-118">Dẫn hướng đến **điều khiển Access (iam)**  >  người **quản trị cổ điển**  >  **Thêm**  >  **Thêm người quản trị đồng** để mở ngăn **Thêm đồng quản trị** (Nếu tùy chọn thêm đồng người quản trị bị vô hiệu hóa, nó sẽ cho biết rằng bạn không có quyền).</span><span class="sxs-lookup"><span data-stu-id="56c95-118">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="56c95-119">Chọn người dùng mà bạn muốn thêm, rồi bấm **Thêm**.</span><span class="sxs-lookup"><span data-stu-id="56c95-119">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="56c95-120">**Tìm hiểu thêm:**</span><span class="sxs-lookup"><span data-stu-id="56c95-120">**Learn more:**</span></span>
- [<span data-ttu-id="56c95-121">Thêm người đồng quản trị</span><span class="sxs-lookup"><span data-stu-id="56c95-121">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="56c95-122">Loại bỏ người đồng quản trị</span><span class="sxs-lookup"><span data-stu-id="56c95-122">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="56c95-123">Thay đổi người quản trị dịch vụ</span><span class="sxs-lookup"><span data-stu-id="56c95-123">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="56c95-124">Xem người quản trị tài khoản</span><span class="sxs-lookup"><span data-stu-id="56c95-124">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="56c95-125">Quản lý quyền truy nhập bằng cổng thông tin RBAC và Azure</span><span class="sxs-lookup"><span data-stu-id="56c95-125">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="56c95-126">**Thêm/xóa người dùng bằng cách sử dụng Azure Active Directory (quảng cáo)**</span><span class="sxs-lookup"><span data-stu-id="56c95-126">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="56c95-127">Bạn có thể thêm người dùng mới hoặc xóa người dùng hiện có khỏi tổ chức Azure Active Directory (Azure AD):</span><span class="sxs-lookup"><span data-stu-id="56c95-127">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="56c95-128">Để thêm người dùng mới, hãy đăng nhập vào [cổng thông tin Azure](https://ms.portal.azure.com/#home) với tư cách là người quản trị người dùng cho tổ chức.</span><span class="sxs-lookup"><span data-stu-id="56c95-128">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="56c95-129">Chọn **Azure Active Directory**, chọn **người dùng** rồi bấm **người dùng mới**.</span><span class="sxs-lookup"><span data-stu-id="56c95-129">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="56c95-130">Trên trang **người dùng** , điền thông tin bắt buộc.</span><span class="sxs-lookup"><span data-stu-id="56c95-130">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="56c95-131">Bấm **tạo**.</span><span class="sxs-lookup"><span data-stu-id="56c95-131">Click **Create**.</span></span> <span data-ttu-id="56c95-132">Người dùng được tạo và thêm vào đối tượng thuê Azure AD của bạn.</span><span class="sxs-lookup"><span data-stu-id="56c95-132">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="56c95-133">**Tìm hiểu thêm**:</span><span class="sxs-lookup"><span data-stu-id="56c95-133">**Learn more**:</span></span>

- [<span data-ttu-id="56c95-134">Thêm người dùng mới</span><span class="sxs-lookup"><span data-stu-id="56c95-134">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="56c95-135">Xóa người dùng</span><span class="sxs-lookup"><span data-stu-id="56c95-135">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="56c95-136">Thêm hoặc cập nhật thông tin hồ sơ của người dùng bằng cách sử dụng Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="56c95-136">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="56c95-137">**Tài liệu được đề xuất**</span><span class="sxs-lookup"><span data-stu-id="56c95-137">**Recommended documents**</span></span>

- [<span data-ttu-id="56c95-138">Điều khiển truy nhập dựa trên vai trò là gì (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="56c95-138">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="56c95-139">Tìm hiểu các vai trò khác nhau trong Azure</span><span class="sxs-lookup"><span data-stu-id="56c95-139">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="56c95-140">Quyền quản trị vai trò trong Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="56c95-140">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="56c95-141">Hướng dẫn: cấp quyền truy nhập cho người dùng bằng RBAC và cổng thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="56c95-141">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="56c95-142">Khắc phục sự cố RBAC trong Azure</span><span class="sxs-lookup"><span data-stu-id="56c95-142">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="56c95-143">Sắp xếp các tài nguyên của bạn với các nhóm quản lý Azure</span><span class="sxs-lookup"><span data-stu-id="56c95-143">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="56c95-144">Làm thế nào để yêu cầu bản sao hóa đơn Azure qua email</span><span class="sxs-lookup"><span data-stu-id="56c95-144">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="56c95-145">Cách thêm, Cập Nhật hoặc loại bỏ thẻ tín dụng hoặc thẻ ghi nợ khỏi Azure</span><span class="sxs-lookup"><span data-stu-id="56c95-145">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="56c95-146">Quản lý (kích hoạt lại/hủy bỏ/chuyển) đăng ký</span><span class="sxs-lookup"><span data-stu-id="56c95-146">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



