---
title: Xóa đối tượng thuê
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564875"
---
# <a name="delete-tenant"></a><span data-ttu-id="c0640-102">Xóa đối tượng thuê</span><span class="sxs-lookup"><span data-stu-id="c0640-102">Delete tenant</span></span>

<span data-ttu-id="c0640-103">Để xóa một Azure AD, hãy đảm bảo:</span><span class="sxs-lookup"><span data-stu-id="c0640-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="c0640-104">Bạn là người quản trị toàn cầu trên thư mục.</span><span class="sxs-lookup"><span data-stu-id="c0640-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="c0640-105">Bạn không đăng nhập bằng tài khoản có thư mục mặc định, chẳng hạn như contoso.onmicrosoft.com trong tài khoản đã đăng nhập, chẳng hạn như admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="c0640-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="c0640-106">Loại bỏ mọi ứng dụng hiện hoạt trong thư mục trước khi xóa.</span><span class="sxs-lookup"><span data-stu-id="c0640-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="c0640-107">Để loại bỏ các ứng dụng hiện hoạt, hãy dẫn hướng đến đăng ký ứng dụng và loại bỏ các ứng dụng hiện có.</span><span class="sxs-lookup"><span data-stu-id="c0640-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="c0640-108">Không có đăng ký hiện hoạt nào đối với bất kỳ dịch vụ Microsoft Online nào, chẳng hạn như Microsoft Azure, Office 365 hoặc Azure AD Premium liên kết trên thư mục.</span><span class="sxs-lookup"><span data-stu-id="c0640-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="c0640-109">Chuyển các đăng ký của bạn hoặc đẩy nhanh việc hủy bỏ các đăng ký hiện hoạt thông qua Azure support và thanh toán.</span><span class="sxs-lookup"><span data-stu-id="c0640-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="c0640-110">Tìm hiểu thêm về cách hủy bỏ đăng ký Office 365 và Azure.</span><span class="sxs-lookup"><span data-stu-id="c0640-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="c0640-111">Để được hướng dẫn liên kết hoặc thêm đăng ký hiện có vào một đối tượng thuê, hãy xem [liên kết hoặc thêm đăng ký Azure vào đối tượng thuê AZURE AD của bạn](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="c0640-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="c0640-112">Không có giấy phép hiện hoạt.</span><span class="sxs-lookup"><span data-stu-id="c0640-112">There are no Active license.</span></span> <span data-ttu-id="c0640-113">Để loại bỏ giấy phép, hãy xem [làm thế nào để loại bỏ đăng ký để loại bỏ giấy phép](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="c0640-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="c0640-114">Không có người dùng hiện hoạt nào khác trong thư mục bên cạnh mình là người quản trị toàn cầu khi cố gắng xóa Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c0640-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="c0640-115">Loại bỏ bất kỳ người dùng hiện hoạt nào khác và bất kỳ phụ thuộc nào trong tên miền tùy chỉnh trong đối tượng thuê cũng sẽ cần bị loại bỏ, chẳng hạn như người dùng được tạo bằng admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="c0640-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="c0640-116">Để biết thêm các bước chi tiết về cách thức:</span><span class="sxs-lookup"><span data-stu-id="c0640-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="c0640-117">Xóa bỏ "Azure Active Directory" hoặc "đăng ký", hãy xem [xóa Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="c0640-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="c0640-118">Loại bỏ các ứng dụng trong thư mục, hãy xem [loại bỏ các ứng dụng](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="c0640-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
