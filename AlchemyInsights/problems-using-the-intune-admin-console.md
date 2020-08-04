---
title: Sự cố bằng cách sử dụng bảng điều khiển dành cho quản trị viên InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555883"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="5a710-102">Sự cố bằng cách sử dụng bảng điều khiển dành cho quản trị viên InTune</span><span class="sxs-lookup"><span data-stu-id="5a710-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="5a710-103">**"Truy cập bị từ chối" khi điều hướng cổng quản trị InTune.**</span><span class="sxs-lookup"><span data-stu-id="5a710-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="5a710-104">Nếu bạn là thành viên của vai trò tùy chỉnh InTune, hãy đảm bảo giấy phép InTune hoặc Enterprise Mobility Suite (EMS) được gán cho tài khoản của bạn.</span><span class="sxs-lookup"><span data-stu-id="5a710-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="5a710-105">Nếu bạn đang sử dụng trình quản lý cấu hình để quản lý thiết bị, xác minh bạn không phải là một phần của bộ sưu tập người dùng InTune Configuration Manager MDM.</span><span class="sxs-lookup"><span data-stu-id="5a710-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="5a710-106">Xác minh rằng bạn đã được gán quyền kiểm soát quản trị dựa trên vai trò thích hợp (RBAC) trong vai trò InTune.</span><span class="sxs-lookup"><span data-stu-id="5a710-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="5a710-107">Xác minh nhóm được sử dụng không phải là danh sách phân phối.</span><span class="sxs-lookup"><span data-stu-id="5a710-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="5a710-108">InTune trong cổng thông tin Azure chỉ hỗ trợ tài khoản người dùng thuộc nhóm bảo mật Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5a710-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="5a710-109">Đánh giá nhóm của bạn trong cổng Azure > **InTune**  >  **nhóm**hoặc Azure cổng > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="5a710-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="5a710-110">**Người dùng có quá nhiều quyền cho vai trò InTune được chỉ định**</span><span class="sxs-lookup"><span data-stu-id="5a710-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="5a710-111">Tư vấn cho người dùng để đi đến **InTune**  >  **InTune vai trò**  >  **của tôi cho phép**  >  **xuất** để xem xét cấp quyền.</span><span class="sxs-lookup"><span data-stu-id="5a710-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="5a710-112">**Tôi đã thêm một nhóm phạm vi vào một vai trò, nhưng người dùng trong vai trò đó vẫn nhìn thấy người dùng hoặc thiết bị khác.**</span><span class="sxs-lookup"><span data-stu-id="5a710-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="5a710-113">Phạm vi nhóm không lọc ra người dùng hoặc thiết bị.</span><span class="sxs-lookup"><span data-stu-id="5a710-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="5a710-114">Phạm vi Nhóm:</span><span class="sxs-lookup"><span data-stu-id="5a710-114">Scope groups:</span></span>

- <span data-ttu-id="5a710-115">Giới hạn người dùng có thể gán chính sách hoặc ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="5a710-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="5a710-116">Chỉ cho phép người dùng cụ thể chạy tác vụ từ xa trên thiết bị.</span><span class="sxs-lookup"><span data-stu-id="5a710-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="5a710-117">Để biết thêm thông tin về phạm vi nhóm, xem [kiểm soát truy cập Dựa trên vai trò (RBAC) với Microsoft InTune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="5a710-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="5a710-118">**Tôi đã thêm người dùng vào vai trò InTune nhưng họ vẫn có quyền truy cập đầy đủ vào bảng điều khiển dành cho quản trị viên InTune.**</span><span class="sxs-lookup"><span data-stu-id="5a710-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="5a710-119">Điều hướng đến InTune > **người dùng** trong cổng thông tin Azure và xác minh rằng người dùng không được gán cho bất kỳ vai trò sau đây trong cổng Azure:</span><span class="sxs-lookup"><span data-stu-id="5a710-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="5a710-120">Quản trị viên toàn cầu</span><span class="sxs-lookup"><span data-stu-id="5a710-120">Global administrator</span></span>
- <span data-ttu-id="5a710-121">Quản trị viên dịch vụ InTune</span><span class="sxs-lookup"><span data-stu-id="5a710-121">Intune service administrator</span></span>
- <span data-ttu-id="5a710-122">Quản trị viên SharePoint</span><span class="sxs-lookup"><span data-stu-id="5a710-122">SharePoint administrator</span></span>

<span data-ttu-id="5a710-123">Để biết thêm thông tin, xem [kiểm soát truy cập Dựa trên vai trò (RBAC) với Microsoft InTune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="5a710-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="5a710-124">**Vấn đề truy cập**</span><span class="sxs-lookup"><span data-stu-id="5a710-124">**Access Issues**</span></span>

<span data-ttu-id="5a710-125">Để biết thêm thông tin, [hãy xem bạn không thể đăng nhập vào Office 365, Azure hoặc InTune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="5a710-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>