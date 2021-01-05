---
title: Cách thêm và quản lý người quản trị
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755533"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="78f51-102">Cách thêm và quản lý người quản trị</span><span class="sxs-lookup"><span data-stu-id="78f51-102">How to add and manage admins</span></span>

<span data-ttu-id="78f51-103">Dựa trên mô tả vấn đề của bạn, chúng tôi đã tìm ra giải pháp cho bạn.</span><span class="sxs-lookup"><span data-stu-id="78f51-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="78f51-104">Hầu hết khách hàng đều có thể giải quyết được sự cố của họ sau khi theo dõi tài liệu hướng dẫn của chúng tôi.</span><span class="sxs-lookup"><span data-stu-id="78f51-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="78f51-105">Để quản lý tài khoản thanh toán của bạn cho thỏa thuận khách hàng của Microsoft (MCA), bạn có thể sử dụng các vai trò khác nhau với mức truy nhập mong muốn.</span><span class="sxs-lookup"><span data-stu-id="78f51-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="78f51-106">Những vai trò này cũng cộng với các vai trò dịch vụ Azure tích hợp sẵn giúp bạn điều khiển các tài nguyên của mình.</span><span class="sxs-lookup"><span data-stu-id="78f51-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="78f51-107">**Để thêm vai trò thanh toán trong cổng thông tin Azure:**</span><span class="sxs-lookup"><span data-stu-id="78f51-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="78f51-108">Đăng nhập vào [cổng thông tin Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="78f51-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="78f51-109">Tìm kiếm *quản lý chi phí + thanh toán*.</span><span class="sxs-lookup"><span data-stu-id="78f51-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="78f51-110">Chọn Access Control (IAM) ở một phạm vi như tài khoản thanh toán, Hồ sơ thanh toán hoặc phần hóa đơn mà bạn muốn cấp quyền truy nhập.</span><span class="sxs-lookup"><span data-stu-id="78f51-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="78f51-111">Trang điều khiển Access (IAM) liệt kê những người dùng và nhóm được gán cho từng vai trò cho phạm vi đó.</span><span class="sxs-lookup"><span data-stu-id="78f51-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="78f51-112">Để cấp quyền truy nhập cho người dùng, hãy chọn **Thêm** từ phía trên cùng của trang.</span><span class="sxs-lookup"><span data-stu-id="78f51-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="78f51-113">Trong danh sách thả xuống *vai trò* , hãy chọn một vai trò.</span><span class="sxs-lookup"><span data-stu-id="78f51-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="78f51-114">Nhập địa chỉ email của người dùng mà bạn muốn cấp quyền truy nhập.</span><span class="sxs-lookup"><span data-stu-id="78f51-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="78f51-115">Chọn **lưu** để gán vai trò.</span><span class="sxs-lookup"><span data-stu-id="78f51-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="78f51-116">Để loại bỏ quyền truy nhập cho người dùng, hãy chọn người dùng có gán vai trò mà bạn muốn loại bỏ.</span><span class="sxs-lookup"><span data-stu-id="78f51-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="78f51-117">Chọn **loại bỏ**.</span><span class="sxs-lookup"><span data-stu-id="78f51-117">Select **Remove**.</span></span>

<span data-ttu-id="78f51-118">**Tài liệu được đề xuất**</span><span class="sxs-lookup"><span data-stu-id="78f51-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="78f51-119">Định nghĩa vai trò thanh toán</span><span class="sxs-lookup"><span data-stu-id="78f51-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="78f51-120">Các vai trò và nhiệm vụ của tài khoản thanh toán</span><span class="sxs-lookup"><span data-stu-id="78f51-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="78f51-121">Bắt đầu với tài khoản thanh toán MCA của bạn</span><span class="sxs-lookup"><span data-stu-id="78f51-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="78f51-122">Kiểm tra quyền truy nhập vào thỏa thuận khách hàng của Microsoft</span><span class="sxs-lookup"><span data-stu-id="78f51-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
