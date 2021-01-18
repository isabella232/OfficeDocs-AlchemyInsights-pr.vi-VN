---
title: Gán nhóm tới Azure AD Role
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
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885403"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="b10bd-102">Gán nhóm tới Azure AD Role</span><span class="sxs-lookup"><span data-stu-id="b10bd-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="b10bd-103">Để gán một nhóm Azure AD với nguồn chính quyền trong Azure AD thành vai trò Azure AD, hãy thực hiện các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="b10bd-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="b10bd-104">Tạo nhóm mới-để tạo nhóm mới:</span><span class="sxs-lookup"><span data-stu-id="b10bd-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="b10bd-105">một.</span><span class="sxs-lookup"><span data-stu-id="b10bd-105">a.</span></span> <span data-ttu-id="b10bd-106">Đăng nhập vào Trung tâm quản trị Azure AD với **người quản trị vai trò đặc quyền** hoặc quyền **người quản trị toàn cầu** .</span><span class="sxs-lookup"><span data-stu-id="b10bd-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="b10bd-107">b.</span><span class="sxs-lookup"><span data-stu-id="b10bd-107">b.</span></span> <span data-ttu-id="b10bd-108">Chọn **các nhóm > Azure Active Directory > tất cả các nhóm > nhóm mới**.</span><span class="sxs-lookup"><span data-stu-id="b10bd-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="b10bd-109">c's.</span><span class="sxs-lookup"><span data-stu-id="b10bd-109">c.</span></span> <span data-ttu-id="b10bd-110">Tạo nhóm.</span><span class="sxs-lookup"><span data-stu-id="b10bd-110">Create the group.</span></span>

2. <span data-ttu-id="b10bd-111">Gán vai trò cho nhóm trong khi tạo nhóm hoặc sau khi nhóm được tạo.</span><span class="sxs-lookup"><span data-stu-id="b10bd-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="b10bd-112">một.</span><span class="sxs-lookup"><span data-stu-id="b10bd-112">a.</span></span> <span data-ttu-id="b10bd-113">Để gán vai trò cho nhóm tại thời điểm tạo nhóm, hãy chuyển đổi trên các **vai trò chuyển đổi AZURE AD có thể được gán cho nhóm** và tạo nhóm.</span><span class="sxs-lookup"><span data-stu-id="b10bd-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="b10bd-114">b.</span><span class="sxs-lookup"><span data-stu-id="b10bd-114">b.</span></span> <span data-ttu-id="b10bd-115">Để gán vai trò cho nhóm sau khi đã được tạo, hãy dẫn hướng đến tab **vai trò được gán** cho nhóm mới được tạo và gán vai trò cho nhóm.</span><span class="sxs-lookup"><span data-stu-id="b10bd-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="b10bd-116">**Quản lý tư cách thành viên của một nhóm được gán cho vai trò Azure AD**</span><span class="sxs-lookup"><span data-stu-id="b10bd-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="b10bd-117">Để ngăn không cho độ cao của đặc quyền, theo mặc định, chỉ người quản trị vai trò đặc quyền và người quản trị toàn cầu có thể sửa đổi tư cách thành viên của một nhóm được gán cho vai trò.</span><span class="sxs-lookup"><span data-stu-id="b10bd-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="b10bd-118">Tuy nhiên, họ có thể chọn gán chủ sở hữu cho một nhóm và đại diện cho nhiệm vụ này.</span><span class="sxs-lookup"><span data-stu-id="b10bd-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="b10bd-119">Để biết thêm chi tiết về việc gán nhóm điện toán đám mây thành Azure vai trò, hãy xem mục [gán vai trò quảng cáo cho nhóm điện toán đám mây](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="b10bd-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="b10bd-120">Để biết thêm chi tiết về các vai trò khắc phục sự cố được gán cho nhóm đám mây, hãy xem [khắc phục các vai trò được gán cho nhóm đám mây](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="b10bd-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





