---
title: Các vấn đề khi sử dụng bảng điều khiển quản trị InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728309"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="93510-102">Các vấn đề khi sử dụng bảng điều khiển quản trị InTune</span><span class="sxs-lookup"><span data-stu-id="93510-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="93510-103">**"Access bị từ chối" khi dẫn hướng đến cổng thông tin quản trị InTune.**</span><span class="sxs-lookup"><span data-stu-id="93510-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="93510-104">Nếu bạn là thành viên của một vai trò tùy chỉnh InTune, hãy đảm bảo giấy phép InTune hoặc gói phần mềm di động (EMS) được gán cho tài khoản của bạn.</span><span class="sxs-lookup"><span data-stu-id="93510-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="93510-105">Nếu bạn đang sử dụng trình quản lý cấu hình để quản lý thiết bị, hãy xác nhận bạn không phải là một phần của tuyển tập người dùng InTune cho MDM trình quản lý cấu hình.</span><span class="sxs-lookup"><span data-stu-id="93510-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="93510-106">Xác nhận rằng bạn đã được gán quyền điều khiển quản trị dựa trên vai trò thích hợp (RBAC) cho phép trong lưỡi InTune vai trò.</span><span class="sxs-lookup"><span data-stu-id="93510-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="93510-107">Xác nhận nhóm được sử dụng không phải là danh sách phân phối.</span><span class="sxs-lookup"><span data-stu-id="93510-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="93510-108">InTune trong cổng thông tin Azure chỉ hỗ trợ các tài khoản người dùng thuộc về các nhóm bảo mật Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="93510-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="93510-109">Xem lại các nhóm của bạn trong cổng thông tin Azure > **InTune**  >  **nhóm**hoặc trong Azure Portal > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="93510-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="93510-110">**Người dùng có quá nhiều quyền đối với vai trò InTune được gán**</span><span class="sxs-lookup"><span data-stu-id="93510-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="93510-111">Thông báo cho người dùng để đi đến **InTune**điều  >  **chỉnh vai trò**  >  **của tôi**  >  **xuất** quyền để xem lại quyền được cấp.</span><span class="sxs-lookup"><span data-stu-id="93510-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="93510-112">**Tôi đã thêm một nhóm phạm vi vào vai trò, nhưng người dùng trong vai trò đó vẫn nhìn thấy những người dùng hoặc thiết bị khác.**</span><span class="sxs-lookup"><span data-stu-id="93510-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="93510-113">Nhóm phạm vi không lọc ra người dùng hoặc thiết bị.</span><span class="sxs-lookup"><span data-stu-id="93510-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="93510-114">Nhóm phạm vi:</span><span class="sxs-lookup"><span data-stu-id="93510-114">Scope groups:</span></span>

- <span data-ttu-id="93510-115">Giới hạn người dùng có thể gán các chính sách hoặc ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="93510-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="93510-116">Chỉ cho phép người dùng cụ thể chạy các tác vụ từ xa trên các thiết bị.</span><span class="sxs-lookup"><span data-stu-id="93510-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="93510-117">Để biết thêm thông tin về các nhóm phạm vi, hãy xem  [kiểm soát truy nhập dựa trên vai trò (RBAC) với Microsoft InTune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="93510-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="93510-118">**Tôi đã thêm một người dùng vào vai trò InTune nhưng vẫn có quyền truy nhập đầy đủ vào bảng điều khiển quản trị InTune.**</span><span class="sxs-lookup"><span data-stu-id="93510-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="93510-119">Dẫn hướng đến InTune > **người dùng** trong cổng thông tin Azure và xác nhận rằng người dùng không được gán cho bất kỳ vai trò nào sau đây trong cổng thông tin Azure:</span><span class="sxs-lookup"><span data-stu-id="93510-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="93510-120">Người quản trị toàn cầu</span><span class="sxs-lookup"><span data-stu-id="93510-120">Global administrator</span></span>
- <span data-ttu-id="93510-121">Người quản trị dịch vụ InTune</span><span class="sxs-lookup"><span data-stu-id="93510-121">Intune service administrator</span></span>
- <span data-ttu-id="93510-122">Người quản trị SharePoint</span><span class="sxs-lookup"><span data-stu-id="93510-122">SharePoint administrator</span></span>

<span data-ttu-id="93510-123">Để biết thêm thông tin, hãy xem [kiểm soát truy nhập dựa trên vai trò (RBAC) với Microsoft InTune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="93510-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="93510-124">**Vấn đề truy nhập**</span><span class="sxs-lookup"><span data-stu-id="93510-124">**Access Issues**</span></span>

<span data-ttu-id="93510-125">Để biết thêm thông tin, hãy xem [bạn không thể đăng nhập vào Office 365, Azure hoặc InTune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="93510-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>