---
title: Chuyển quyền sở hữu thanh toán Azure
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
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922239"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="5afd0-102">Chuyển quyền sở hữu thanh toán Azure</span><span class="sxs-lookup"><span data-stu-id="5afd0-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="5afd0-103">Đăng nhập vào [cổng thông tin Azure](https://portal.azure.com/) với tư cách là người quản trị của tài khoản thanh toán có đăng ký mà bạn muốn chuyển.</span><span class="sxs-lookup"><span data-stu-id="5afd0-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="5afd0-104">Nếu bạn không chắc chắn nếu bạn là người quản trị, hoặc nếu bạn cần xác định ai, hãy xem [xác định người quản trị thanh toán tài khoản](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="5afd0-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="5afd0-105">Tìm kiếm về **quản lý chi phí + thanh toán**.</span><span class="sxs-lookup"><span data-stu-id="5afd0-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="5afd0-106">Chọn **đăng ký** từ ngăn bên trái.</span><span class="sxs-lookup"><span data-stu-id="5afd0-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="5afd0-107">Tùy thuộc vào quyền truy nhập, bạn có thể cần phải chọn một phạm vi thanh toán, sau đó **thuê** bao hoặc **đăng ký Azure**.</span><span class="sxs-lookup"><span data-stu-id="5afd0-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="5afd0-108">Chọn **chuyển quyền sở hữu thanh toán** cho thuê bao mà bạn muốn chuyển</span><span class="sxs-lookup"><span data-stu-id="5afd0-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="5afd0-109">Nhập địa chỉ email của người dùng là người quản trị thanh toán của tài khoản đó sẽ là chủ sở hữu mới cho đăng ký, rồi chọn **gửi yêu cầu chuyển**</span><span class="sxs-lookup"><span data-stu-id="5afd0-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="5afd0-110">Người dùng nhận được một email với các hướng dẫn để xem lại yêu cầu chuyển của bạn.</span><span class="sxs-lookup"><span data-stu-id="5afd0-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="5afd0-111">Để phê duyệt yêu cầu chuyển, người dùng sẽ chọn liên kết trong email và làm theo hướng dẫn.</span><span class="sxs-lookup"><span data-stu-id="5afd0-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="5afd0-112">**Lưu ý** : nếu bạn chuyển quyền sở hữu thanh toán của gói đăng ký của mình vào tài khoản của người dùng trong một đối tượng thuê Azure AD khác, tất cả các [điều khiển truy nhập dựa trên vai trò (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)để quản lý tài nguyên trong đăng ký đều bị loại bỏ vĩnh viễn.</span><span class="sxs-lookup"><span data-stu-id="5afd0-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="5afd0-113">Chỉ có chủ sở hữu mới sẽ có quyền truy nhập để quản lý tài nguyên trong đăng ký.</span><span class="sxs-lookup"><span data-stu-id="5afd0-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="5afd0-114">Để biết thêm thông tin, hãy xem mục [chuyển gói đăng ký cho người dùng trong một đối tượng thuê AZURE AD khác](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="5afd0-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="5afd0-115">**Tài liệu được đề xuất**</span><span class="sxs-lookup"><span data-stu-id="5afd0-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="5afd0-116">Chuyển quyền sở hữu thanh toán của một thuê bao Azure sang một tài khoản khác</span><span class="sxs-lookup"><span data-stu-id="5afd0-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="5afd0-117">Giới thiệu về việc chuyển quyền sở hữu thanh toán cho một thuê bao Azure</span><span class="sxs-lookup"><span data-stu-id="5afd0-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="5afd0-118">Chuyển giao Visual Studio, mạng Microsoft Partner (MPN) và trả tiền theo mức sử dụng cho các thuê bao dev/Test</span><span class="sxs-lookup"><span data-stu-id="5afd0-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="5afd0-119">Chuyển câu hỏi về quyền sở hữu</span><span class="sxs-lookup"><span data-stu-id="5afd0-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="5afd0-120">Khắc phục sự cố về quyền sở hữu truyền</span><span class="sxs-lookup"><span data-stu-id="5afd0-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
