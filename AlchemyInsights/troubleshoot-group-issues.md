---
title: Khắc phục sự cố nhóm
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "50714442"
---
# <a name="troubleshoot-group-issues"></a><span data-ttu-id="396cd-102">Khắc phục sự cố nhóm</span><span class="sxs-lookup"><span data-stu-id="396cd-102">Troubleshoot group issues</span></span>

<span data-ttu-id="396cd-103">**Tôi cần gán một nhóm cho vai trò Azure AD**</span><span class="sxs-lookup"><span data-stu-id="396cd-103">**I need to assign a group to an Azure AD role**</span></span>

<span data-ttu-id="396cd-104">Để gán nhóm Azure Active Directory (AD) vào vai trò Azure AD, hãy thực hiện các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="396cd-104">To assign an Azure Active Directory (AD) group to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="396cd-105">Tạo nhóm mới-để tạo nhóm mới:</span><span class="sxs-lookup"><span data-stu-id="396cd-105">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="396cd-106">một.</span><span class="sxs-lookup"><span data-stu-id="396cd-106">a.</span></span> <span data-ttu-id="396cd-107">Đăng nhập vào Trung tâm quản trị Azure AD với người quản trị vai trò đặc quyền hoặc quyền người quản trị toàn cầu.</span><span class="sxs-lookup"><span data-stu-id="396cd-107">Sign in to the Azure AD admin center with privileged role administrator or global administrator permissions.</span></span> 
    <span data-ttu-id="396cd-108">b.</span><span class="sxs-lookup"><span data-stu-id="396cd-108">b.</span></span> <span data-ttu-id="396cd-109">Chọn các nhóm > Azure Active Directory > tất cả các nhóm > nhóm mới.</span><span class="sxs-lookup"><span data-stu-id="396cd-109">Select Azure Active Directory > Groups > All groups > New group.</span></span> 
    <span data-ttu-id="396cd-110">c's.</span><span class="sxs-lookup"><span data-stu-id="396cd-110">c.</span></span> <span data-ttu-id="396cd-111">Tạo nhóm.</span><span class="sxs-lookup"><span data-stu-id="396cd-111">Create the group.</span></span>

2. <span data-ttu-id="396cd-112">Gán vai trò cho nhóm trong khi tạo nhóm hoặc sau khi nhóm được tạo.</span><span class="sxs-lookup"><span data-stu-id="396cd-112">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="396cd-113">một.</span><span class="sxs-lookup"><span data-stu-id="396cd-113">a.</span></span> <span data-ttu-id="396cd-114">Để gán vai trò cho nhóm tại thời điểm tạo nhóm, hãy chuyển đổi trên các vai trò chuyển đổi Azure AD có thể được gán cho nhóm và tạo nhóm.</span><span class="sxs-lookup"><span data-stu-id="396cd-114">To assign a role to the group at the time of group creation, switch on the toggle Azure AD roles can be assigned to the group and create the group.</span></span>
    <span data-ttu-id="396cd-115">b.</span><span class="sxs-lookup"><span data-stu-id="396cd-115">b.</span></span> <span data-ttu-id="396cd-116">Để gán vai trò cho nhóm sau khi đã được tạo, hãy dẫn hướng đến tab vai trò được gán cho nhóm mới được tạo và gán vai trò cho nhóm.</span><span class="sxs-lookup"><span data-stu-id="396cd-116">To assign a role to the group after it has been created, navigate to the Assigned roles tab for the newly created group, and assign the role to the group.</span></span>

<span data-ttu-id="396cd-117">**Tôi cần quản lý tư cách thành viên của một nhóm được gán cho vai trò Azure AD**</span><span class="sxs-lookup"><span data-stu-id="396cd-117">**I need to manage membership of a group that is assigned to Azure AD role**</span></span>

1. <span data-ttu-id="396cd-118">Để ngăn không cho độ cao của đặc quyền, theo mặc định, chỉ người quản trị vai trò đặc quyền và người quản trị toàn cầu có thể sửa đổi tư cách thành viên của một nhóm được gán cho vai trò.</span><span class="sxs-lookup"><span data-stu-id="396cd-118">To prevent elevation of privileges, by default, only privileged role administrator and global administrator can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="396cd-119">Tuy nhiên, họ có thể chọn gán chủ sở hữu cho một nhóm và đại diện cho nhiệm vụ này.</span><span class="sxs-lookup"><span data-stu-id="396cd-119">They can, however, choose to assign an owner for such a group and delegate this task.</span></span> <span data-ttu-id="396cd-120">Để biết thêm thông tin hãy xem, [sử dụng các nhóm đám mây để quản lý việc gán vai trò trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="396cd-120">For more information see, [Use cloud groups to manage role assignments in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span>
2. <span data-ttu-id="396cd-121">Đối với các câu hỏi thường gặp và mẹo khắc phục sự cố gán vai trò cho các nhóm trong Azure AD, hãy xem các [vai trò khắc phục sự cố được gán cho nhóm điện toán đám mây](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="396cd-121">For common questions and troubleshooting tips for assigning roles to groups in Azure AD, see [Troubleshooting roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>

<span data-ttu-id="396cd-122">**Nhóm động**</span><span class="sxs-lookup"><span data-stu-id="396cd-122">**Dynamic groups**</span></span>

1. <span data-ttu-id="396cd-123">Nếu bạn không thể tìm thấy thuộc tính người dùng tích hợp sẵn, hãy đảm bảo rằng thuộc tính nằm trong danh sách các thuộc tính được hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="396cd-123">If you cannot find the built-in user attributes, ensure that the attribute is in the list of supported properties.</span></span>
2. <span data-ttu-id="396cd-124">Nếu bạn đang tìm kiếm các thuộc tính thiết bị tích hợp sẵn, hãy đảm bảo rằng thuộc tính nằm trong danh sách thuộc tính của thiết bị</span><span class="sxs-lookup"><span data-stu-id="396cd-124">If you are looking for built-in device attributes, ensure that the attribute is in the list of device attributes</span></span> 
3. <span data-ttu-id="396cd-125">Ngoài các thuộc tính người dùng và thiết bị tích hợp sẵn, bạn cũng có thể sử dụng [thuộc tính phần mở rộng](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties).</span><span class="sxs-lookup"><span data-stu-id="396cd-125">In addition to the built-in user and device attributes, you could also use [Extension Attributes](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties).</span></span> <span data-ttu-id="396cd-126">Sau khi đồng bộ hóa các thuộc tính của phần mở rộng từ quảng cáo Windows Server tại cơ sở hoặc từ một ứng dụng SaaS được kết nối, các thuộc tính sẽ được hiển thị trong danh sách thả xuống của bộ dựng quy tắc.</span><span class="sxs-lookup"><span data-stu-id="396cd-126">After syncing extension attributes from on-premises Windows Server AD or from a connected SaaS application, the attributes should be visible in the drop-down list of the rule builder.</span></span> <span data-ttu-id="396cd-127">Có thể tìm thấy tên thuộc tính tùy chỉnh trong thư mục bằng cách truy vấn thuộc tính của người dùng bằng PowerShell và tìm kiếm tên thuộc tính.</span><span class="sxs-lookup"><span data-stu-id="396cd-127">The custom attribute name can be found in the directory by querying a user's attribute using PowerShell and searching for the attribute name.</span></span> <span data-ttu-id="396cd-128">Những điều này cũng có thể sử dụng khi xây dựng các quy tắc trong cú pháp quy tắc.</span><span class="sxs-lookup"><span data-stu-id="396cd-128">These could also be used when constructing rules in the rule syntax.</span></span>
4. <span data-ttu-id="396cd-129">Đảm bảo rằng đối tượng thuê của bạn có giấy phép thích hợp.</span><span class="sxs-lookup"><span data-stu-id="396cd-129">Ensure that your tenant has the appropriate license.</span></span> <span data-ttu-id="396cd-130">Các nhóm động yêu cầu người thuê để có giấy phép Azure AD P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="396cd-130">Dynamic groups require the tenant to have an Azure AD P1 Premium license.</span></span> <span data-ttu-id="396cd-131">Danh sách các gói giấy phép Azure AD có thể được truy nhập [tại đây](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="396cd-131">The list of Azure AD license plans can be accessed [here](https://azure.microsoft.com/pricing/details/active-directory/).</span></span> <span data-ttu-id="396cd-132">Có thể truy nhập các gói cấp phép doanh nghiệp + tính bảo mật [tại đây](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing).</span><span class="sxs-lookup"><span data-stu-id="396cd-132">Enterprise Mobility + Security licensing plans can be accessed [here](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing).</span></span>
5. <span data-ttu-id="396cd-133">Đảm bảo vai trò của người dùng tạo nhóm động là người quản trị toàn cầu, người quản trị InTune, người quản trị nhóm hoặc người quản trị người dùng.</span><span class="sxs-lookup"><span data-stu-id="396cd-133">Ensure that the role of the user creating the dynamic group is a global administrator, intune administrator, group administrator, or a user administrator.</span></span>
6. <span data-ttu-id="396cd-134">Xin vui lòng cho phép thời gian nhóm để định cư.</span><span class="sxs-lookup"><span data-stu-id="396cd-134">Please allow time for the group to populate.</span></span> <span data-ttu-id="396cd-135">Tùy thuộc vào kích cỡ của đối tượng thuê của bạn, nhóm có thể mất đến 24 giờ để tổng hợp lần đầu tiên hoặc sau khi có một quy tắc thay đổi.</span><span class="sxs-lookup"><span data-stu-id="396cd-135">Depending on the size of your tenant, the group may take up to 24 hours for populating for the first time or after a rule change.</span></span>
7. <span data-ttu-id="396cd-136">Để biết thêm thông tin, hãy xem [tạo quy tắc dựa trên thuộc tính cho tư cách thành viên nhóm động](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).</span><span class="sxs-lookup"><span data-stu-id="396cd-136">For more information, see [Create attribute-based rules for dynamic group membership](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).</span></span>

<span data-ttu-id="396cd-137">**Tôi cần xóa nhóm**</span><span class="sxs-lookup"><span data-stu-id="396cd-137">**I need to delete a group**</span></span>

1. <span data-ttu-id="396cd-138">Nhóm có thể bị xóa khỏi thư mục bằng cách sử dụng lệnh ghép ngắn Remove-AzureADGroup trong mô-đun Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="396cd-138">Groups can be deleted from the directory using the Remove-AzureADGroup cmdlet in the Azure AD Powershell module.</span></span>
2. <span data-ttu-id="396cd-139">Trước khi tìm cách xóa một nhóm đã đồng bộ trong Azure AD, hãy đảm bảo rằng bạn đã xóa tất cả giấy phép đã gán để tránh lỗi.</span><span class="sxs-lookup"><span data-stu-id="396cd-139">Before attempting to delete a synced group in Azure AD, ensure you have deleted all assigned licenses  to avoid errors.</span></span>
3. <span data-ttu-id="396cd-140">Để biết thêm thông tin về việc xóa nhóm, hãy xem mục [xóa một nhóm với giấy phép đã gán](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).</span><span class="sxs-lookup"><span data-stu-id="396cd-140">For more information on deleting groups, see [Deleting a group with an assigned license](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).</span></span>

<span data-ttu-id="396cd-141">**Tôi cần khôi phục nhóm đã xóa**</span><span class="sxs-lookup"><span data-stu-id="396cd-141">**I need to restore a deleted group**</span></span>

1. <span data-ttu-id="396cd-142">Nếu nhóm Office 365 bị xóa, chỉ có thể khôi phục được tối đa 30 ngày trước khi xóa vĩnh viễn.</span><span class="sxs-lookup"><span data-stu-id="396cd-142">If an Office 365 group is deleted, it can only be restored up to 30 days before permanent deletion occurs.</span></span> <span data-ttu-id="396cd-143">Sau khi bị xóa vĩnh viễn, nhóm không còn được khôi phục.</span><span class="sxs-lookup"><span data-stu-id="396cd-143">Once permanently deleted, the group can no longer be restored.</span></span> <span data-ttu-id="396cd-144">Tìm hiểu thêm về việc khôi phục các nhóm [ở đây](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span><span class="sxs-lookup"><span data-stu-id="396cd-144">Learn more about restoring groups [here](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>
2. <span data-ttu-id="396cd-145">Chức năng này không được hỗ trợ đối với nhóm bảo mật và nhóm phân phối.</span><span class="sxs-lookup"><span data-stu-id="396cd-145">This functionality is not supported for security groups and distribution groups.</span></span>
3. <span data-ttu-id="396cd-146">Đảm bảo bạn được ủy quyền để khôi phục một nhóm Office 365.</span><span class="sxs-lookup"><span data-stu-id="396cd-146">Ensure you are authorized to restore an Office 365 group.</span></span> <span data-ttu-id="396cd-147">Người quản trị toàn cầu, người quản trị nhóm, người quản trị tài khoản người dùng, người quản trị dịch vụ InTune, đối tác tier1 hoặc tier2 hỗ trợ và chủ sở hữu của nhóm có thể khôi phục nhóm.</span><span class="sxs-lookup"><span data-stu-id="396cd-147">Global administrators, group administrators, user account administrators, intune service administrators, partner tier1 or tier2 support, and the owner of the group can be able to restore a group.</span></span>
4. <span data-ttu-id="396cd-148">Khi một nhóm đã bị xóa và đã khôi phục, nó được xem như một nhóm mới và đã được tự động điền theo quy tắc.</span><span class="sxs-lookup"><span data-stu-id="396cd-148">When a dynamic group is deleted and restored, it is seen as a new group and re-populated according to the rule.</span></span> <span data-ttu-id="396cd-149">Quá trình này có thể mất đến 24 giờ.</span><span class="sxs-lookup"><span data-stu-id="396cd-149">This process might take up to 24 hours.</span></span>
5. <span data-ttu-id="396cd-150">Để biết thêm thông tin về việc khôi phục một nhóm đã xóa, hãy xem [khôi phục nhóm Office đã xóa 365 trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span><span class="sxs-lookup"><span data-stu-id="396cd-150">For more information on restoring a deleted group, see [Restore a deleted Office 365 group in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>

<span data-ttu-id="396cd-151">**Cấu hình chính sách hết hạn nhóm**</span><span class="sxs-lookup"><span data-stu-id="396cd-151">**Group expiration policy configuration**</span></span>

1. <span data-ttu-id="396cd-152">Chức năng này chỉ được hỗ trợ cho các nhóm Office 365, chứ không phải cho các nhóm bảo mật và nhóm phân phối không được hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="396cd-152">This functionality is only supported for Office 365 groups, and not for security groups and distribution groups are not supported.</span></span>
2. <span data-ttu-id="396cd-153">Cấu hình và sử dụng chính sách hết hạn cho các nhóm Office 365 yêu cầu giấy phép Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="396cd-153">Configuring and using the expiration policy for Office 365 groups requires an Azure AD Premium license.</span></span>
3. <span data-ttu-id="396cd-154">Hiện tại, chỉ có một chính sách hết hạn có thể được cấu hình cho các nhóm Office 365 trên một đối tượng thuê.</span><span class="sxs-lookup"><span data-stu-id="396cd-154">Currently, only one expiration policy can be configured for Office 365 groups on a tenant.</span></span>
4. <span data-ttu-id="396cd-155">Chỉ có người quản trị toàn cầu, người quản trị nhóm, người quản trị người dùng và chủ sở hữu của nhóm có thể gia hạn một nhóm.</span><span class="sxs-lookup"><span data-stu-id="396cd-155">Only Global administrators, group administrators, user administrators, and the owner of the group can be able to renew a group.</span></span>
5. <span data-ttu-id="396cd-156">Nếu nhóm Office 365 hết hạn, bạn sẽ bị xóa và chỉ có thể khôi phục được tối đa 30 ngày trước khi xóa vĩnh viễn xảy ra.</span><span class="sxs-lookup"><span data-stu-id="396cd-156">If an Office 365 group is expired, it is deleted and can only be restored up to 30 days before permanent deletion occurs.</span></span> <span data-ttu-id="396cd-157">Sau khi bị xóa vĩnh viễn, nhóm không còn được khôi phục.</span><span class="sxs-lookup"><span data-stu-id="396cd-157">Once permanently deleted, the group can no longer be restored.</span></span> <span data-ttu-id="396cd-158">Tìm hiểu thêm về việc khôi phục các nhóm [ở đây](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span><span class="sxs-lookup"><span data-stu-id="396cd-158">Learn more about restoring groups [here](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>

<span data-ttu-id="396cd-159">**Gia hạn tự động dựa trên hoạt động**</span><span class="sxs-lookup"><span data-stu-id="396cd-159">**Activity-based automatic renewal**</span></span>

<span data-ttu-id="396cd-160">Hoạt động của người dùng từ SharePoint, Outlook và nhóm có thể kích hoạt tự động gia hạn nhóm.</span><span class="sxs-lookup"><span data-stu-id="396cd-160">User activities from SharePoint, Outlook and Teams can trigger group automatic renewal.</span></span> <span data-ttu-id="396cd-161">Các hoạt động được kiểm tra tại 35 ngày trước khi nhóm hết hạn.</span><span class="sxs-lookup"><span data-stu-id="396cd-161">Activities are checked at 35 days before a group expires.</span></span> <span data-ttu-id="396cd-162">Nếu có hoạt động trong vòng đời nhóm hiện tại, nhóm sẽ được tự động gia hạn và thông báo email sẽ không được gửi đến người sở hữu nhóm.</span><span class="sxs-lookup"><span data-stu-id="396cd-162">If there is activity during the current group lifecycle, the group will be automatically renewed and email notification won't be sent out to group owners.</span></span>

<span data-ttu-id="396cd-163">**Thời gian thông báo cho các nhóm đã hết hạn**</span><span class="sxs-lookup"><span data-stu-id="396cd-163">**Notification timing for expired groups**</span></span>

1. <span data-ttu-id="396cd-164">Thông báo email được gửi đến chủ sở hữu nhóm 365 của Office 30 ngày, 15 ngày và 1 ngày trước ngày hết hạn của nhóm.</span><span class="sxs-lookup"><span data-stu-id="396cd-164">Email notifications are sent to the Office 365 group owners 30 days, 15 days, and 1 day prior to expiration of the group.</span></span>
2. <span data-ttu-id="396cd-165">Khi bạn thiết lập trước hết hạn, bất kỳ nhóm nào cũ hơn khoảng hết hạn được đặt thành 35 ngày cho đến khi hết hạn.</span><span class="sxs-lookup"><span data-stu-id="396cd-165">When you first set up expiration, any groups that are older than the expiration interval are set to 35 days until expiration.</span></span>
3. <span data-ttu-id="396cd-166">Ngày hết hạn nhóm được tính toán dựa trên ngày gia hạn của nhóm, không dựa vào ngày Cập Nhật chính sách.</span><span class="sxs-lookup"><span data-stu-id="396cd-166">Group expiration date is calculated based on the group’s renewal date, not based on the policy updated date.</span></span> <span data-ttu-id="396cd-167">Nếu Cập Nhật chính sách hết hạn, ngày hết hạn sẽ không thay đổi.</span><span class="sxs-lookup"><span data-stu-id="396cd-167">If the expiration policy is updated, the expiration date will not change.</span></span>
4. <span data-ttu-id="396cd-168">Để biết thêm thông tin, hãy xem, [chính sách hết hạn nhóm và email gia hạn](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) và [khôi phục một nhóm đã xóa Office 365 trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span><span class="sxs-lookup"><span data-stu-id="396cd-168">For more information see, [Group Expiration policy and renewal emails](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) and [Restore a deleted Office 365 group in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>

<span data-ttu-id="396cd-169">**Quyền tạo nhóm**</span><span class="sxs-lookup"><span data-stu-id="396cd-169">**Permission to create a group**</span></span>

<span data-ttu-id="396cd-170">Đảm bảo rằng bạn được ủy quyền để tạo nhóm mới.</span><span class="sxs-lookup"><span data-stu-id="396cd-170">Ensure that you are authorized to create a new group.</span></span> <span data-ttu-id="396cd-171">Người quản trị toàn cầu có thể tắt tính năng tạo nhóm trong cổng thông tin Azure hoặc Pa-nen truy nhập.</span><span class="sxs-lookup"><span data-stu-id="396cd-171">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="396cd-172">Bạn có thể cần người quản trị để tạo nhóm mới cho bạn hoặc để cung cấp cho bạn quyền thích hợp.</span><span class="sxs-lookup"><span data-stu-id="396cd-172">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

1. [<span data-ttu-id="396cd-173">Tạo một nhóm mới và thêm các thành viên trong Azure Portal</span><span class="sxs-lookup"><span data-stu-id="396cd-173">Create a new group and add members in Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [<span data-ttu-id="396cd-174">Tạo nhóm trong PowerShell MSOnline</span><span class="sxs-lookup"><span data-stu-id="396cd-174">Create groups in Powershell MSOnline</span></span>](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [<span data-ttu-id="396cd-175">Tắt tính năng tạo nhóm trong PowerShell</span><span class="sxs-lookup"><span data-stu-id="396cd-175">Disable groups creation in Powershell</span></span>](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [<span data-ttu-id="396cd-176">Quản lý những người có thể tạo nhóm trong Office 365</span><span class="sxs-lookup"><span data-stu-id="396cd-176">Manage who can create groups in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [<span data-ttu-id="396cd-177">Tắt thông báo chào mừng trong Office 365 qua PowerShell</span><span class="sxs-lookup"><span data-stu-id="396cd-177">Disable Office 365 welcome notification via Powershell</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [<span data-ttu-id="396cd-178">Vai trò quản trị Azure AD</span><span class="sxs-lookup"><span data-stu-id="396cd-178">Azure AD administrative roles</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

<span data-ttu-id="396cd-179">**Quản lý quyền tạo nhóm**</span><span class="sxs-lookup"><span data-stu-id="396cd-179">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="396cd-180">Người quản trị toàn cầu có thể quản lý quyền tạo nhóm cho các nhóm bảo mật hoặc Office 365 được tạo trong trang Azure Portal hoặc Pa-nen truy nhập, bằng cách thiết đặt **người dùng có thể tạo nhóm bảo mật trong Azure Portals** hoặc **người dùng có thể tạo nhóm Office 365 trong Azure Portals** cài đặt trong **tất cả các nhóm > chung (thiết đặt)**.</span><span class="sxs-lookup"><span data-stu-id="396cd-180">Global administrators can manage group creation permissions for security or Office 365 groups created in the Azure portal or Access Panel, by setting **Users can create security groups in Azure portals** or **Users can create Office 365 groups in Azure portals** settings in **All groups > General (Settings)**.</span></span>
2. <span data-ttu-id="396cd-181">Bạn cũng có thể hạn chế tạo nhóm để chọn một nhóm người dùng nếu bạn có giấy phép Azure AD P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="396cd-181">You can also restrict group creation to select a group of users if you have an Azure AD P1 Premium license.</span></span>

<span data-ttu-id="396cd-182">**Tắt thông báo chào mừng cho các thành viên mới của một nhóm Office 365**</span><span class="sxs-lookup"><span data-stu-id="396cd-182">**Disabling welcome notification for new members of an Office 365 group**</span></span>

<span data-ttu-id="396cd-183">Thông báo chào mừng được gửi đến những người dùng được thêm vào các nhóm Office 365 có thể bị vô hiệu hóa bằng cách đặt `UnifiedGroupWelcomeMessageEnabled` thành **false** trong PowerShell.</span><span class="sxs-lookup"><span data-stu-id="396cd-183">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting `UnifiedGroupWelcomeMessageEnabled` to **False** in Powershell.</span></span> <span data-ttu-id="396cd-184">Tìm hiểu về thiết đặt này [ở đây](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).</span><span class="sxs-lookup"><span data-stu-id="396cd-184">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).</span></span>












