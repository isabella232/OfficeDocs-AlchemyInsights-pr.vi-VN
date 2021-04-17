---
title: Hóa đơn email Azure hiện đại
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820848"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="5efc6-102">Lập hóa đơn email trong Azure</span><span class="sxs-lookup"><span data-stu-id="5efc6-102">Email invoicing in Azure</span></span>

<span data-ttu-id="5efc6-103">Bạn phải có chủ sở hữu hoặc vai trò đóng góp trên hồ sơ thanh toán hoặc tài khoản thanh toán của nó để cập nhật tùy chọn hóa đơn email của nó.</span><span class="sxs-lookup"><span data-stu-id="5efc6-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="5efc6-104">Sau khi bạn đã chọn tham gia, tất cả người dùng với một chủ sở hữu, người đóng góp, bộ đọc và các vai trò trình quản lý hóa đơn trên hồ sơ thanh toán sẽ nhận được hóa đơn trong email.</span><span class="sxs-lookup"><span data-stu-id="5efc6-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="5efc6-105">Đăng nhập vào [cổng thông tin Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="5efc6-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="5efc6-106">Tìm kiếm **quản lý chi phí + thanh toán**.</span><span class="sxs-lookup"><span data-stu-id="5efc6-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="5efc6-107">Chọn hóa **đơn** từ bên trái, rồi chọn **hóa đơn email** từ phía trên cùng của trang.</span><span class="sxs-lookup"><span data-stu-id="5efc6-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="5efc6-108">Nếu bạn có nhiều hồ sơ thanh toán, hãy chọn một hồ sơ thanh toán, rồi chọn chọn **tham** gia.</span><span class="sxs-lookup"><span data-stu-id="5efc6-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="5efc6-109">Chọn **Cập Nhật**.</span><span class="sxs-lookup"><span data-stu-id="5efc6-109">Select **Update**.</span></span>
6. <span data-ttu-id="5efc6-110">Nếu bạn có nhiều hồ sơ thanh toán, hãy chọn một hồ sơ thanh toán, rồi chọn chọn **tham** gia.</span><span class="sxs-lookup"><span data-stu-id="5efc6-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="5efc6-111">Bạn cung cấp cho người khác quyền truy nhập để xem, tải xuống và thanh toán hóa đơn bằng cách gán vai trò trình quản lý hóa đơn cho hồ sơ thanh toán MCA hoặc MPA.</span><span class="sxs-lookup"><span data-stu-id="5efc6-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="5efc6-112">Nếu bạn đã chọn tham gia để lấy hóa đơn của mình trong email, người dùng cũng sẽ nhận được các hóa đơn trong email.</span><span class="sxs-lookup"><span data-stu-id="5efc6-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="5efc6-113">Đăng nhập vào [cổng thông tin Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="5efc6-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="5efc6-114">Tìm kiếm **quản lý chi phí + thanh toán**.</span><span class="sxs-lookup"><span data-stu-id="5efc6-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="5efc6-115">Chọn **hồ sơ thanh toán** từ bên trái.</span><span class="sxs-lookup"><span data-stu-id="5efc6-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="5efc6-116">Từ danh sách hồ sơ thanh toán, hãy chọn một hồ sơ thanh toán mà bạn muốn gán vai trò trình quản lý hóa đơn.</span><span class="sxs-lookup"><span data-stu-id="5efc6-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="5efc6-117">Chọn **Access Control (iam)** từ bên trái, rồi chọn **Thêm** từ phía trên cùng của trang.</span><span class="sxs-lookup"><span data-stu-id="5efc6-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="5efc6-118">Trong danh sách thả xuống vai trò, chọn **trình quản lý hóa đơn**.</span><span class="sxs-lookup"><span data-stu-id="5efc6-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="5efc6-119">Nhập địa chỉ email của người dùng để cấp quyền truy nhập.</span><span class="sxs-lookup"><span data-stu-id="5efc6-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="5efc6-120">Chọn **lưu** để gán vai trò.</span><span class="sxs-lookup"><span data-stu-id="5efc6-120">Select **Save** to assign the role.</span></span>
